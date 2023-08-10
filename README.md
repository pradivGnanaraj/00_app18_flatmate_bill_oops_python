# Flatmates Bill Calculator and Report Generator

This script calculates how much each flatmate should pay for a bill based on the number of days they stayed in the house during the bill period. It then generates a PDF report displaying the bill breakdown.

## Prerequisites

- Python 3.x
- Install required packages using the following command:

  ```bash
  pip install filestack-python fpdf webbrowser
  ```

## Usage

1. Run the script by executing the following command in your terminal:

   ```bash
   python main_script.py
   ```

2. Input the bill amount and period, along with information about each flatmate's name and number of days they stayed in the house.

3. The script will calculate how much each flatmate needs to pay and generate a PDF report displaying the bill breakdown.

## Project Structure

- `main_script.py`: Main script that takes user inputs, calculates payments, generates PDF report, and shares the report using Filestack.
- `flat.py`: Defines the `Bill` and `Flatmate` classes to manage bill and flatmate data.
- `reports.py`: Contains the `PdfReport` and `FileSharer` classes to generate PDF reports and share files using Filestack.
- `files/`: Folder containing additional files required for the project.
  - `house.png`: Icon used in the PDF report.
  - `design.txt`: A design document or notes related to the project.
  - `bill_report.pdf`: Sample generated PDF report.

## Credits

This project was inspired by the need to fairly divide bills among flatmates based on their stay duration. The `filestack-python` library was used for file sharing and the `fpdf` library for generating PDF reports.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```