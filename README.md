# Good day👋, I wrote a currency converter, and now I’ll tell you about it.

# Currency Converter

This is a simple currency converter web application that allows users to convert between various foreign currencies and Russian Rubles (RUB). The application is built using HTML for the structure, CSS for styling, and JavaScript for the functionality.

## Features

- **User-friendly Interface:** The interface provides a clear and intuitive design for users to input the amount in a selected foreign currency and instantly see the converted amount in Russian Rubles.

- **Currency Selection:** Users can choose the currency they want to convert from and the currency they want to convert to using dropdown menus.

- **Real-time Exchange Rates:** The application fetches real-time exchange rates from the Central Bank of Russia using the [CBR Daily API](https://www.cbr-xml-daily.ru/daily_json.js). The rates are updated once per hour to ensure accuracy.

- **Persistent Settings:** The user's selected currencies are stored in local storage, allowing the application to remember their preferences even after refreshing the page.

## Usage

1. Open the `index.html` file in a web browser.

2. Select the currency you want to convert from in the "From" dropdown menu.

3. Enter the amount you want to convert in the input field next to the "From" currency.

4. The converted amount will be instantly displayed in Russian Rubles in the input field next to the "To" currency.

5. Optionally, you can change the "To" currency to see the equivalent amount in a different foreign currency.

## Code Overview

### HTML Structure

The structure is defined in the `index.html` file, using a form with input fields and dropdown menus for currency selection.

### JavaScript (converter.js)

The `Converter` class manages the conversion process. It includes methods to fetch real-time exchange rates, handle currency changes, and store user preferences in local storage.

The conversion logic is implemented using asynchronous functions and event listeners. The application calculates the converted amount in real-time as users input values or change currency selections.

## Dependencies

- [axios](https://github.com/axios/axios): Used for making HTTP requests to the CBR Daily API.


