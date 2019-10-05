# vott_setup  
Ubuntu16.04にVoTTを導入するための手順  
kernel:4.15.0-64-generic
  
1. Node.jsおよびnpmをインストール(2019/10/05現在、nodejs:v11.15.0、npm:6.7.0が最新)[1]  
> curl -sL https://deb.nodesource.com/setup_11.x | sudo -E bash -  
> sudo apt-get install -y nodejs  
  
2. VoTTをクローンし、npmを使用してセットアップ[2]  
> git clone https://github.com/Microsoft/VoTT.git  
> cd VoTT  
> npm install  
> npm start  
  
2. 足りないと言われたものをインストール[3]  
> npm install popper.js@^1.14.7 --save  
> npm install react-dnd@^5.0.0 --save  
> npm install react-dnd-html5-backend@^3.0.2 --save  
  
3. 古いと言われたものをアップグレード[4]
> npm install core-js@3 --save  
> npm update caniuse-lite browserslist
> npm install fsevents@1.2.9 --save  
> npm i -f  
> npm audit fix  
  
<参考文献>  
[1]http://idwonder21.hatenablog.com/entry/2019/02/06/103423  
[2]https://www.kinacon-blog.work/entry/2019/03/16/VoTT%E3%81%A7%E5%AD%A6%E7%BF%92%E7%94%A8%E3%83%87%E3%83%BC%E3%82%BF%E3%82%BB%E3%83%83%E3%83%88%E3%82%92%E4%BD%9C%E6%88%90%E3%81%99%E3%82%8B  
[3]https://stackoverflow.com/questions/47039812/how-to-install-popper-js-with-bootstrap-4  
[4]https://stackoverflow.com/questions/40226745/npm-warn-notsup-skipping-optional-dependency-unsupported-platform-for-fsevents  