# cocos2d-x
## HelloWorld

### 委托类头文件
```c++
#ifndef  _APP_DELEGATE_H_
#define  _APP_DELEGATE_H_

#include "cocos2d.h"

// 私有继承application 意味着只能在这个类中调用application里的函数不能使用对象调用application里的函数
class  AppDelegate : private cocos2d::Application
{
public:
    AppDelegate();
    virtual ~AppDelegate();

    virtual void initGLContextAttrs();

    /**
    *	游戏启动时调用的函数，在这里可以初始化导演对象和场景对象
    */
	
    virtual bool applicationDidFinishLaunching();

    /**
    *	游戏进入后台时调用的函数
    */
	
    virtual void applicationDidEnterBackground();

    /**
    *	游戏进入前台时调用的函数
    */
	
    virtual void applicationWillEnterForeground();
};

#endif // _APP_DELEGATE_H_
    
```

### 委托类实现
```c++

```