# 使用 JB, CKAN API on depositor
## Some notes on using JB and CKAN on depositor

1. Install JupyterBook (JB) on my local machine (Mac OS 13.5/ M1)
    * Quickly kickstart using terminal cmd line : 
    ```
    % jb create hello-hello-book
    % jb build .
    % cd _build/html
    % python -m http.server 8000 # preview on browser
    ```


     * High level JB creating process
        1. Create content
        2. Build
        3. Publish 
    
    * Structure of JB 
        * _config.yml：book configuration
        * _toc.yml：toc of book 
        * content/*.md or .ipynb：content of book

        
2. Use CKAN API on depositar
>API token: (hidden)

    * (🔨) 上傳到資料樣本到 depositar 
    * (✅) 與 depositar 的 API 串接與查詢結果
    * (✅）在頁面中呈現資料集內容

