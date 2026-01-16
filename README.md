# Currency Converter

A simple, user-friendly web application that allows you to convert amounts between different world currencies in real-time.

![Currency Converter Preview](./pics/preview.png) <!-- Add a screenshot of your app if available -->

## Features

- Real-time currency conversion using live exchange rates
- Intuitive user interface with currency dropdowns
- Automatic flag updates based on selected currencies
- Responsive design that works on all devices
- Instant conversion on page load and on button click
- Support for multiple world currencies

## How It Works

The Currency Converter uses the [Frankfurter API](https://www.frankfurter.dev/) to fetch real-time exchange rates. The application:

1. Allows users to select "from" and "to" currencies from dropdown menus
2. Accepts an input amount to convert
3. Fetches current exchange rates from the API
4. Calculates and displays the converted amount
5. Updates country flags based on selected currencies

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- [Frankfurter API](https://www.frankfurter.dev/) for exchange rates
- [Flags API](https://www.flagcdn.com/) for country flags

## Installation

1. Clone or download this repository to your local machine
2. Open the `index.html` file in your preferred web browser
3. The currency converter will load with default currency pair (USD to INR)

Alternatively, you can host it on a local server:

```bash
# Navigate to the project directory
cd Currency_Converter

# Start a simple server (if Python is installed)
python -m http.server 8000

# Or for Python 2
python -m SimpleHTTPServer 8000
```

Then open `http://localhost:8000` in your browser.

## Usage

1. Select the currency you want to convert from in the first dropdown
2. Select the currency you want to convert to in the second dropdown
3. Enter the amount you wish to convert
4. Click the "Convert" button or simply wait for automatic conversion
5. The converted amount will be displayed in the message area

## Program Details

The Currency Converter application consists of three main files:

- **index.html**: Contains the structure of the application with:
  - An amount input field
  - Two dropdowns for selecting "from" and "to" currencies
  - Country flag images that update based on selected currencies
  - A message area to display conversion results
  - A convert button

- **style.css**: Provides styling for the application with:
  - A pleasant color scheme (light yellow background with green button)
  - Responsive layout using flexbox
  - Proper spacing and alignment
  - Visual feedback for interactive elements

- **app.js**: Implements the core functionality:
  - Fetches exchange rates from Frankfurter API
  - Updates flag images based on selected currencies
  - Performs currency conversion calculations
  - Handles user interactions and form submission

- **codes.js**: Contains a mapping of currency codes to country codes for flag display

## API

This application uses the Frankfurter API which provides:
- No API key required
- CORS-enabled for browser requests
- Real-time exchange rates for most world currencies
- Base currency defaults to EUR, but can be changed

## Customization

You can easily customize this currency converter:

- Add more currencies by updating the `countryList` in `codes.js`
- Change default currencies in the JavaScript code
- Modify the styling in `style.css`
- Update the conversion logic in `app.js`

## Known Limitations

- Some less common currencies may not be supported by the API
- Conversion rates update in real-time but may have slight delays
- Requires an internet connection to fetch current exchange rates

## Project Structure

```
Currency_Converter/
│
├── index.html          # Main HTML structure
├── style.css           # Styling and layout
├── app.js              # Main application logic
├── codes.js            # Currency codes and countries mapping
└── README.md           # Project documentation
```

## Contributing

Contributions are welcome! Here are some ways you can contribute:

1. Report bugs and issues
2. Suggest new features
3. Improve documentation
4. Submit pull requests for bug fixes or enhancements

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Thanks to [Frankfurter API](https://www.frankfurter.dev/) for providing free real-time exchange rates
- Flags provided by [FlagCDN](https://flagcdn.com/)