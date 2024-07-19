# AI-Based Resume Screening Application

4. Place the AI models generated from Google Colab into the `models` directory.

### Running the Application

1. Start the Flask server:

   ```bash
   flask run
   ```

2. Open your browser and navigate to `http://127.0.0.1:5000/`.

### Usage

- Upload your resume in TXT or PDF format.
- The application will process the resume and display categorized information, job recommendations, and parsed details such as name, phone number, email, skills, and education.

## Directory Structure

```
resume-screening-app/
│
├── models/                   # Directory to store AI models
│
├── static/
│   ├── css/                  # CSS files for styling
│   └── js/                   # JavaScript files (if any)
│
├── templates/                # HTML templates for Flask
│   └── index.html
│
├── app.py                    # Main Flask application
│
├── requirements.txt          # List of required packages
│
└── README.md                 # This README file
```

## Contributing

Contributions are welcome! Please fork this repository and submit pull requests.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contact

If you have any questions or suggestions, feel free to contact me at printekgraphicske@gmail.com

---

Feel free to customize the README file according to your specific needs and information.





consider this 


InconsistentVersionWarning: Trying to unpickle estimator DecisionTreeClassifier from version 1.3.2 when using version 1.5.0. This might lead to breaking code or invalid results. Use at your own risk. For more info please refer to:
https://scikit-learn.org/stable/model_persistence.html#security-maintainability-limitations


use this guide to escape this errors 



The `InconsistentVersionWarning` you're seeing is due to a version mismatch between the version of `scikit-learn` used when the model was pickled (1.3.2) and the version currently installed (1.5.0). This could potentially lead to issues with the model's behavior or results.

Here are a few approaches to address this:

1. **Upgrade/Downgrade `scikit-learn`**: If possible, install the version of `scikit-learn` that matches the version used when the model was saved. You can use the following command to install a specific version:

   ```bash
   pip install scikit-learn==1.3.2
   ```

2. **Re-train the Model**: If you have the original training data and code, the best approach might be to re-train the model using the current version of `scikit-learn` (1.5.0). This ensures compatibility and that you're using the latest features and fixes.

3. **Model Refactoring**: If re-training is not an option, you could try refactoring the code to adapt to the new version. However, this may require significant changes depending on the nature of the version incompatibility.

4. **Test Thoroughly**: If you decide to use the model with the new version despite the warning, make sure to thoroughly test the model to ensure it behaves as expected and produces valid results.

5. **Consult Documentation**: The [scikit-learn documentation](https://scikit-learn.org/stable/model_persistence.html#security-maintainability-limitations) provides guidance on handling such warnings and potential risks associated with model version mismatches.

Which approach works best will depend on your specific circumstances, such as whether you have access to the original training data or if upgrading/downgrading the library is feasible.







