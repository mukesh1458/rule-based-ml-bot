# Face-api.js Models

The files for the pre-trained models used by `face-api.js` are not included in this repository due to their size. You need to download them and place them in this directory for the emotion detection to work correctly.

## Instructions

1.  **Download the Models:**
    You can download the model files from the `face-api.js` GitHub repository. A convenient way is to download the entire `weights` folder from the repository.

    You can find the files here:
    [https://github.com/justadudewhohacks/face-api.js/tree/master/weights](https://github.com/justadudewhohacks/face-api.js/tree/master/weights)

2.  **Download and Place Files:**
    Download all the files from the `weights` directory linked above.

3.  **Place them in this directory (`/public/models`):**
    Once downloaded, place all the model files (`*.json` and `*.weights`) directly into this `/public/models` folder. The final file structure in your project should look like this:

    ```
    public/
    ├── models/
    │   ├── ssd_mobilenetv1_model-weights_manifest.json
    │   ├── ssd_mobilenetv1_model-shard1
    │   ├── face_landmark_68_model-weights_manifest.json
    │   ├── face_landmark_68_model-shard1
    │   ├── face_expression_model-weights_manifest.json
    │   ├── face_expression_model-shard1
    │   └── ... and so on for all models
    └── ... other public files
    ```

After placing the files here, restart the application, and the emotion detection should load correctly.
