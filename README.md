# CoinMarketCap Clone

A simplified clone of the CoinMarketCap cryptocurrency dashboard focusing on displaying cryptocurrency pricing and volume data.


## Overview

This project is a lightweight, educational implementation of a cryptocurrency dashboard inspired by CoinMarketCap. It's built with HTML and Tailwind CSS, focusing on displaying the most important price and volume data for the top cryptocurrencies.

## Features

- Responsive design that works on mobile and desktop
- Dark theme matching CoinMarketCap's interface
- Interactive table with hover effects
- Display of key cryptocurrency metrics:
  - Current prices
  - 24-hour trading volume
  - 24-hour price change percentages
- Navigation and filter UI elements

## Technologies Used

- HTML5
- [Tailwind CSS](https://tailwindcss.com/) (via CDN)
- Responsive design principles
- Custom color theming

## Getting Started

1. Clone this repository
   ```
   git clone https://github.com/lewismosage/assessment-project.git
   ```

2. Open `index.html` in your browser
   - No build process required as Tailwind CSS is loaded via CDN

## Customization

### Adding More Cryptocurrencies

To add more cryptocurrencies to the table, duplicate the table row structure in the HTML file:

```html
<tr class="border-b border-light-blue hover:bg-light-blue">
    <td class="py-4 pl-4 pr-2">11</td>
    <td class="py-4 px-2">
        <div class="flex items-center">
            <div class="w-8 h-8 rounded-full bg-purple-500 flex items-center justify-center mr-3">
                <span class="text-white font-bold">C</span>
            </div>
            <div>
                <div class="font-medium">Coin Name</div>
                <div class="text-xs text-gray-400">SYMBOL</div>
            </div>
        </div>
    </td>
    <td class="py-4 px-2 text-right font-medium">$0.00</td>
    <td class="py-4 px-2 text-right text-accent-green">+0.00%</td>
    <td class="py-4 px-2 text-right">
        <div>$0,000,000</div>
        <div class="text-xs text-gray-400">0.00 SYMBOL</div>
    </td>
</tr>
```

### Changing the Color Theme

To modify the color theme, update the Tailwind configuration in the `<head>` section:

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                'dark-blue': '#0d1421',
                'medium-blue': '#1e2a3b',
                'light-blue': '#2c3b4e',
                'accent-blue': '#3861fb',
                'accent-green': '#16c784',
                'accent-red': '#ea3943',
            }
        }
    }
}
```

## Production Use

For production:

1. Install Tailwind CSS via npm and configure a build process
2. Set up real-time API integration with a cryptocurrency data provider
3. Implement state management for filters and sorting

## License

This project was developed as part of an assessment task. All cryptocurrency data is placeholder information.

## Acknowledgements

- Design inspired by [CoinMarketCap](https://coinmarketcap.com/)
- Icons and styling based on cryptocurrency industry standards
