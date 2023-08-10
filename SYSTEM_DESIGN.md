**Components:**

1. **User Interface (UI):**
   - The user interacts with the program through the command-line interface (CLI).
   - The CLI prompts the user to input bill details and flatmate information.

2. **Main Script (`main_script.py`):**
   - Acts as the main controller of the application.
   - Takes user inputs for bill amount, period, and flatmate details.
   - Calculates individual payments based on stay days using the `Flatmate` class.
   - Generates PDF reports using the `PdfReport` class.
   - Shares the generated report using the `FileSharer` class.

3. **Flatmate Class (`flat.py`):**
   - Represents a flatmate and their stay duration.
   - Computes the amount each flatmate owes based on their stay days.

4. **PdfReport Class (`reports.py`):**
   - Handles the generation of PDF reports.
   - Utilizes the FPDF library to create a PDF file.
   - Embeds relevant details such as the bill period, flatmate names, and calculated payments.

5. **FileSharer Class (`reports.py`):**
   - Uses the Filestack API to upload and share the generated PDF report.
   - Generates a shareable link to the uploaded report.

6. **External Files (`files/`):**
   - Contains additional resources such as icons, design documents, and sample generated reports.

**Flow:**

1. The user provides input through the CLI, including the bill amount, period, and flatmate information.

2. The main script processes the input, calculates individual payments, and generates a PDF report using the PdfReport class.

3. The PdfReport class creates a PDF file with relevant information and stores it in the `files/` directory.

4. The FileSharer class uses the Filestack API to upload the generated PDF report to the cloud.

5. The FileSharer class generates a shareable link to the uploaded report.

6. The user can access the shareable link to view and download the PDF report.

**Benefits:**

- Simplifies the process of splitting shared bills among flatmates.
- Generates clear and organized PDF reports for transparency.
- Promotes efficient communication and understanding among flatmates.
- Demonstrates Python coding skills, use of external libraries, and file handling expertise.
