**Receptionist Chatbot**

**Introduction**

This Python chatbot serves as a virtual receptionist for Company, offering customer support functionalities through a user-friendly interface. It leverages spaCy for intent recognition and interacts with customers via text-based prompts.

**Features**

- **Order Placement:** Guides customers through placing orders for development, consulting, or support services, potentially integrating with order processing systems in a production environment.
- **Appointment Scheduling:** Schedules appointments with the appropriate department based on availability and sends confirmation emails. Currently uses a placeholder mechanism for scheduling, but can be integrated with calendar APIs.
- **Complaint Filing:** Allows customers to submit complaints, capturing details like severity and optionally saving them to a CSV file for tracking.
- **Information Retrieval:** Provides company hours, location/contact details, and basic product information. Can be extended to incorporate product catalogs or knowledge bases.
- **Other Inquiries:** Enables customers to ask questions and potentially receive answers via email (optional).

**Prerequisites**

- **Python 3:** The primary programming language.
- **Required Libraries:** Install them using `pip install`:
    - `spaCy`: Provides natural language processing capabilities.
    - `csv`: Handles CSV file operations for data persistence (complaints and inquiries).
    - `datetime`: Used for date and time manipulation in various functionalities.
    - `email`: Facilitates email communication for appointment confirmations (replace with a more robust solution like `smtplib` for production).

**Instructions**

1. **Install Libraries:** Use `pip install <library_name>` for each required library.
2. **Replace Placeholders:**
    - Update `company_name` (line 4) to reflect your company's name.
    - Replace email credentials in `COMPANY_EMAIL` and `COMPANY_EMAIL_PASSWORD` (lines 27, 28) with your actual company email and password (consider more secure methods in production).
    - Replace placeholder values in schedule_appointment (lines 55-60) with logic for appointment availability and department determination.
    - Update company address, phone number, and email in get_information (lines 102-104) with your company's details.

**Important Note:**

The current email sending functionality uses a placeholder mechanism and may not be suitable for production environments. Explore more secure solutions using libraries like `smtplib` or cloud-based email APIs.

**Running the Chatbot**

1. Save the code as a Python file (e.g., `receptionist_chatbot.py`).
2. Open a terminal or command prompt.
3. Navigate to the directory containing the file.
4. Run the script using: `python receptionist_chatbot.py`

**Disclaimer**

This is a demonstration chatbot template. Adapt and extend its functionalities to suit your specific business needs. For production use, enhance security measures (e.g., data validation, secure email communication, user authentication).

**Future Enhancements**

- Integrate with order processing systems for real-time order fulfillment.
- Connect with calendar APIs for appointment scheduling.
- Implement more robust intent recognition using spaCy or other NLP libraries.
- Design a more interactive user interface (e.g., web-based chatbot) for broader reach.
- Add functionalities based on your specific customer service needs.

**Feedback and Contributions**

Feel free to submit issues or pull requests on GitHub to improve this project.
