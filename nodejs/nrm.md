##使用nrm快速切换npm源

####使用nrm快速切换npm源

nrm 是一个 NPM 源管理器，允许你快速地在如下 NPM 源间切换：

列表项目
    - npm
    - cnpm
    - strongloop
    - enropean
    - australia
    - nodejitsu
    - taobao


####Install

npm install -g nrm

####列出可用的源

nrm list

  npm ---- https://registry.npmjs.org/
  cnpm --- http://r.cnpmjs.org/
  taobao - http://registry.npm.taobao.org/
  eu ----- http://registry.npmjs.eu/
  au ----- http://registry.npmjs.org.au/
  sl ----- http://npm.strongloop.com/
  nj ----- https://registry.nodejitsu.com/
  pt ----- http://registry.npmjs.pt/


####切换

nrm use taobao

####增加源

nrm add <registry> <url> [home]

####删除源

nrm del <registry>

####测试速度

nrm test










































