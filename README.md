* Step 1: Clone the Repository
First, clone the repository to your local machine.
Navigate into the project directory: cd coalesce
* Step 2: Install Dependencies
```bash
  npm install
```

* Step 3: Split the OpenAPI Specification
To split your OpenAPI swagger.json file into smaller files for easier maintenance, you can use the ReDoc CLI split command.
Run the following command:
```bash
  redocly split swagger.json --outDir=./openapi
```
This will split your swagger.json into multiple files and save them in the openapi directory.
* Step 4: Serve the Documentation Locally
  ```bash 
  redocly preview-docs ./openapi/coalesce.json
  ```
* Step 5: Optional Customizations
You can customize the OpenAPI specification further by modifying the coalesce.json file in the ./openapi directory.
Any changes you make will be reflected the next time you run the preview.
* Step 6: Commit and Push Your Changes
   ```bash 
  git add .
  git commit -m "Setup ReDoc project with coalesce.json"
  git push origin main
  ```
Step 7: Future Changes
If you update your OpenAPI specification, repeat the split and preview steps, making sure to keep the name as coalesce.json.


