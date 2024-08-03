Hey guys, welcome to my repository. Before, you start working on this app, I would like to provide you some prerequisite steps that needs to be done.

Prerequisite steps:
1. Since the app runs using stable diffusion v1.4, Since the model is huge in order to download this we require a library called git-lfs(large file system). you can find this in this link https://git-lfs.com/ .
2. After downloading git-lfs, follow the steps from https://docs.github.com/en/repositories/working-with-files/managing-large-files/installing-git-large-file-storage .
3. After successfully initiating git-lfs, you can download the model using this command git clone  "https://huggingface.co/CompVis/stable-diffusion-v1-4" .
4. We need to build a new image from an existing image in order to add this file. To do so, just use this command docker compose up --build  in cmd.
5. It would take time to build this image. In the meantime, we can uncomment some lines in the code to make this application successfully running. the lines that needs uncommenting are 12,13,31,32,33.
6. That's it when the image is built successfully, you can access this application either by 172.0.0.1:8000 or localhost:8000. There you go now you have diffuse-me app ready.
