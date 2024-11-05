# psexec_noinstall
The repository contains psexec, which will help to exploit the forgotten pipe

Have a non-genius administrator connect using PsExec to the host:
![изображение](https://user-images.githubusercontent.com/92790655/220080852-9588a359-b413-4b75-86ef-dc177aa59f55.png)


We discovered this when we saw the RemCom_Communication bundle. This one is standard for PsExec
![изображение](https://user-images.githubusercontent.com/92790655/220081012-c10148d6-4aef-4951-86b8-efe769d52fb7.png)


Using psexec_noinstall, it is possible to connect to this pipeline as any low-privileged user, since the DACL of the pipeline allows this:
![изображение](https://user-images.githubusercontent.com/92790655/220081419-fe45e1b0-c57a-4f10-9f61-9b6345443e87.png)
![изображение](https://user-images.githubusercontent.com/92790655/220082245-f3f4c66f-d3c7-4d7b-af5f-07fb69a47ee5.png)


Here's a checker:

https://github.com/beaverdreamer/nxc-modules
