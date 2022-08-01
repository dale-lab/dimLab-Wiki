# Running the IF Diaphragm analysis pipeline

1. Open <code>VSCode</code>
2. load the modules by pressing <code>Shift+Enter</code> on the first line of the code block
3. Start napari with all the plugins you need by pressing <code>Shift+Enter</code> on the second line of the code block

**First View**
<a> <img alt="Start" src="_media/_pipelines/diaphragm_pipeline/main.png"/> </a>

4. Go to path and select one of the files inside of the folder with all your Channels and press <code>Load Image</code>
<a> <img alt="Start" src="_media/_pipelines/diaphragm_pipeline/img_loaded.png"/> </a>

5. On the right side press <code>Find Sample</code>. you will see a mask covering your sample
<a> <img alt="Start" src="_media/_pipelines/diaphragm_pipeline/find_sample.png"/> </a>

6. If the mask is correct proceed to press <code>Extract Clean Image</code>. You will see how the background is remove from your sample.
<a> <img alt="Start" src="_media/_pipelines/diaphragm_pipeline/sample_extracted.png"/> </a>

7. Finally proceed to selected the correct image (The one that has been cleaned) and press <code>Cellpose</code>. This will give you the detected individual fibers in the sample using cellpose.
<a> <img alt="Start" src="_media/_pipelines/diaphragm_pipeline/find_fibers.png"/> </a>
 