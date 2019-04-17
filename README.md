# 优化APK

1.svg   app:srcCompat <br/>
2.着色器  android:tint="@color/colorAccent" <br/>
3.资源打包配置 resConfigs('zh-rCN') <br/>
4.动态库的打包配置 sourceSets {<br/>
                  main{<br/>
                      jniLibs.srcDirs = ['libs']<br/>
                  }<br/>
              }<br/>
              ndk{<br/>
                          abiFilters('armeabi')//只引入armeabi目录下的so库<br/>
                      }<br/>

5.移除无用资源（Lint）不过是一中物理上的删除<br/>
6.开启代码混淆<br/>
7.启用资源压缩混淆<br/>
8.webp<br/>
9.资源的混淆。7z的压缩，对齐<br/>