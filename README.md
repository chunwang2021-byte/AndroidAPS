
## How to Build
## 如何编译

### If your are familiar with Android development:
* Fork this repository.
* Replace `keystore/demokeystore.jks` with your own key store file.
* Add below secrets in the  `Actions secrets and variables` settings of your repository.  
<a href="/Documentation/screen1.png"><img src="/Documentation/screen1.png?raw=true" alt="Screenshot of Actions secrets" width="800"></a>  
  `KEY_ALIAS`:  Key alais of your key store file.
  `KEY_PASSWORD`: key password of your key store file.
  `STORE_FILE`: Path of your key store file in your repository.
  `STORE_PASSWORD`: Store password of your key store file.
* Trigger build in Github Actions
* Download the `aaps.zip` file in `Artifacts`

### 如果你熟悉安卓开发：
* 克隆此代码仓库到你自己的Github账号
* 用你自己的安卓签名文件替换你克隆的仓库中的`keystore/demokeystore.jks`
* 在你克隆的仓库设置中的  `Actions secrets and variables` 选项中添加如下秘密环境变量：  
<a href="/Documentation/screen1.png"><img src="/Documentation/screen1.png?raw=true" alt="Screenshot of Actions secrets" width="800"></a>  
  `KEY_ALIAS`:  你的安卓签名文件的key alias。
  `KEY_PASSWORD`: 你的安卓签名文件的key密码。
  `STORE_FILE`: 你的安卓签名文件的路径。
  `STORE_PASSWORD`: 你的安卓签名文件的store密码。
* 在Github Actions中触发编译
* 下载`Artifacts`中的编译产物`aaps.zip` 

### If your are NOT familiar with Android development:
You need to get the secerts of the key store file to sign your application. For security reason, all of the passwords are NOT in this repoitory.
**It's really recommanded that you can sign your apk file with your own key store file after learning some Android knowledge.**
Please follow these steps:
* Fork this repository.
* 在你克隆的仓库设置中的  `Actions secrets and variables` 选项中添加如下秘密环境变量：  
<a href="/Documentation/screen1.png"><img src="/Documentation/screen1.png?raw=true" alt="Screenshot of Actions secrets" width="800"></a>  
  `KEY_ALIAS`, `KEY_PASSWORD`, `STORE_FILE`, `STORE_PASSWORD`，这些变量的值都在群中。
* 在Github Actions中触发编译
* 下载`Artifacts`中的编译产物`aaps.zip`
