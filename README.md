# 优化APK

1.svg   app:srcCompat
2.着色器  android:tint="@color/colorAccent"
3.资源打包配置 resConfigs('zh-rCN')
4.动态库的打包配置 sourceSets {
                  main{
                      jniLibs.srcDirs = ['libs']
                  }
              }
              ndk{
                          abiFilters('armeabi')//只引入armeabi目录下的so库
                      }

5.移除无用资源（Lint）不过是一中物理上的删除
6.开启代码混淆
7.启用资源压缩混淆
8.webp
9.资源的混淆。7z的压缩，对齐