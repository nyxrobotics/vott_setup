# vott_setup  
  
1. Node.jsおよびnpmをインストール(2019/10/05現在、nodejs:v11.15.0、npm:6.7.0が最新)[1]  
> curl -sL https://deb.nodesource.com/setup_$(VERSION).x | sudo -E bash -  
> sudo apt-get install -y nodejs  
  
2. VoTTをクローンし、npmを使用してセットアップ[2]  
> git clone https://github.com/Microsoft/VoTT.git  
> cd VoTT  
> npm install  
> npm start  
  
<参考文献>  
[1]http://idwonder21.hatenablog.com/entry/2019/02/06/103423  
[2]https://www.kinacon-blog.work/entry/2019/03/16/VoTT%E3%81%A7%E5%AD%A6%E7%BF%92%E7%94%A8%E3%83%87%E3%83%BC%E3%82%BF%E3%82%BB%E3%83%83%E3%83%88%E3%82%92%E4%BD%9C%E6%88%90%E3%81%99%E3%82%8B  