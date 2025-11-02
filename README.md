# Barcode Decoder Suite

A comprehensive barcode decoding solution supporting multiple barcode formats including PDF417, MaxiCode, QR codes, Aztec codes, and standard barcodes. This project provides Python scripts to decode various barcode types using the ZXing ("Zebra Crossing") barcode image processing library.

## Supported Barcode Types

- PDF417
- MaxiCode
- QR Code
- Aztec Code
- Standard Barcodes (UPC-A, EAN-13, Code 128, etc.)
- Data Matrix

## Prerequisites

- Python 3.6 or higher
- OpenCV (`pip install opencv-python`)
- NumPy (`pip install numpy`)
- Java Runtime Environment (JRE) 8 or higher
- Docker (for some decoders)

## Project Structure

```
├── QRcode_decoder/         # QR Code decoder implementation
│   ├── qrcode_decoder.py
│   └── qrcode.png
├── aztech_decoder/         # Aztec code decoder
│   ├── decode_aztech.py
│   └── aztech-code.png
├── barcode_decoder/        # Standard barcode decoder
│   ├── barcode_decoder.py
│   └── barcode.png
├── maxicode-decoder/       # MaxiCode decoder
│   ├── decode_maxicode.py
│   └── maxicode.png
├── data_matrix_decoder.py  # Data Matrix decoder
├── decode_barcode.py       # Main barcode decoder script
└── requirements.txt        # Python dependencies
```

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd pdf417_decoder
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have Docker installed for the barcode decoder (optional for some decoders)

## Usage

### Decoding Barcodes

1. Place your barcode image in the project directory
2. Run the appropriate decoder script:

   - For standard barcodes:
     ```bash
     python decode_barcode.py
     ```
   
   - For QR codes:
     ```bash
     python QRcode_decoder/qrcode_decoder.py
     ```
   
   - For MaxiCode:
     ```bash
     python maxicode-decoder/decode_maxicode.py
     ```
   
   - For Aztec codes:
     ```bash
     python aztech_decoder/decode_aztech.py
     ```
   
   - For Data Matrix:
     ```bash
     python data_matrix_decoder.py
     ```

## Dependencies

- OpenCV
- NumPy
- ZXing (included in the repository)
- Docker (for some decoders)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- [ZXing (Zebra Crossing)](https://github.com/zxing/zxing) - Barcode image processing library
- [OpenCV](https://opencv.org/) - Computer vision library
- [NumPy](https://numpy.org/) - Numerical computing library

## Troubleshooting

- Ensure all JAR files are in the correct location
- Verify that the input image is clear and the barcode is properly visible
- Check that Docker is running if using the barcode decoder
- Make sure the image file name matches the one specified in the script

## Example Images

Example barcode images are provided in each decoder's directory for testing purposes.
