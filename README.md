# Labelr
QR Code Generator and Printer

A modern, responsive web application for generating and printing QR codes, built with JavaScript and Tailwind CSS.

![labelr mascot](images/labelr.png)
## Features

- Generate QR codes from text or URLs
- Real-time QR code preview
- Customizable QR code size (128x128, 256x256, 512x512)
- Optional title for the QR code
- Print-optimized layout (4x6 inch format)
- Input validation with character limit checking
- Responsive design for all device sizes
- URL parameter support for direct QR code generation

## Technical Stack

- **Frontend Framework**: SolidJS / ECMA 2024 (future)
- **CSS Framework**: Tailwind CSS
- **QR Code Library**: qrcode.js
- **Architecture**: Single Page Application (SPA)

## Implementation Details

### Current Implementation (PoC)
The proof of concept is implemented as a client-side only application with the following features:

- **State Management**: Uses native JavaScript for state handling
- **Real-time Updates**: Implements debounced input handling for efficient QR code generation
- **Print Optimization**: Custom print styles for 4x6 inch format (Chrome only at this point)
- **Error Handling**: Input validation with character limit (191 characters)
- **Responsive Design**: Mobile-first approach using Tailwind CSS

### Future Enhancements

1. **Architecture Migration**
   - Move to MVC architecture
   - Implement proper routing
   - Separate concerns into components
   - Add service layer for business logic

2. **Backend Integration**
   - Add API endpoints for QR code operations
   - Implement database storage for QR codes
   - Add user authentication
   - Enable QR code history and management

3. **Additional Features**
   - Custom color options
   - Error correction level selection
   - QR code template system
   - Batch generation capabilities
   - Export in multiple formats

## Usage

1. Enter text or URL in the input field
2. (Optional) Add a title for the QR code
3. Select desired QR code size
4. Click "Generate QR Code" or wait for auto-generation
5. Click "Print QR Code" to print in 4x6 format

### URL Parameters

The application supports direct QR code generation through URL parameters:

```
https://your-domain.com/?text=Your+Text+Here
```

## Development Setup

none yet...
## Print Specifications

The application is optimized for 4x6 inch printing with the following specifications:

- Page size: 4in x 6in
- Margins: 0
- Content centering: Both vertical and horizontal
- Print-specific styling for optimal output

My current target for this is the Rollo printer.

## Technical Considerations

### Character Limits
- Maximum text length: 191 characters
- Real-time validation
- Helpful error messages

### Performance Optimizations
- Debounced input handling
- Efficient DOM updates
- Print layout optimization

### Browser Compatibility
- Modern browser support
- Fallback handling for older browsers
- Responsive design for all screen sizes

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

[MIT License](LICENSE)

## Support

For issues and feature requests, please use the GitHub issue tracker.