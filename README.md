# cocos2d-x-ImGui
Fixed version from coi version

###Features:
* Programable pipline
* Add ImageButton create with SpriteFrameCached
* Fix Cocos2d-x Implement
* Auto add ImGUI layer on top whenever create or change Scene
* All ImGUI v1.4.8 WIP features + Simple Style Change

###Using: 

1, Replace AppDelegate

2, Add ImGUI functions on any where
```c++
CCIMGUI::getInstance()->addImGUI([=](){
  ImGui::SetNextWindowPos(ImVec2(650, 20), ImGuiSetCond_FirstUseEver);
  ImGui::ShowTestWindow(&isShowDemo);
}, "Function ID");
```
this will auto add to pipline

3, Remove ImGUI functions
```c++
CCIMGUI::getInstance()->removeImGUI("Function ID");
```

4, Other
```c++
CCIMGUI::getInstance()->getWindow() \\ Return GLFWwindow*
CCIMGUI::getInstance()->setShowStyleEditor(true or false)
```

###Preview:
![Preview](https://raw.githubusercontent.com/namkazt/cocos2d-x-ImGui/master/preview.png)
