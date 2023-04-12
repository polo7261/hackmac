# Rocky Linux 9 用 Docker 來安裝WordPress 

[![hackmd-github-sync-badge](https://hackmd.io/BuyfT59LToG_iIU95wR_Pw/badge)](https://hackmd.io/BuyfT59LToG_iIU95wR_Pw)


要在Rocky Linux 9上使用Docker安裝WordPress，您可以按照以下步驟進行操作：

安裝Docker：您需要安裝Docker，可以在終端機上輸入以下命令進行安裝：


sudo dnf install docker
啟動Docker服務：安裝完成後，請啟動Docker服務，可以在終端機上輸入以下命令：


sudo systemctl start docker
下載WordPress映像檔：請使用以下命令從Docker Hub下載WordPress映像檔：


sudo docker pull wordpress
建立WordPress容器：使用以下命令創建一個名為my-wordpress的容器，將WordPress映像檔映射到本地端口8080：

sudo docker run --name my-wordpress -p 8080:80 -d wordpress
訪問WordPress：在瀏覽器上訪問http://localhost:8080，您應該可以看到WordPress安裝頁面。


這裡我要修改一下！