# Android_learning
安卓学习中收集到的知识点和ios之间的区别，持续更新中

安卓初级：

  第一章：安卓常用UI组件

  2025.09.02

1.安卓中线性布局常用代码：
  android:id：
  @+id/login_user：为EditText设置了一个唯一的ID，以便在Java或Kotlin代码中引用它。
  
  android:layout_width：
  match_parent：使EditText的宽度与其父布局的宽度相匹配。
  
  android:layout_height：
  wrap_content：使EditText的高度刚好足够包裹其内容。
  
  android:layout_gravity：
  center：将EditText在其父布局中居中放置（水平方向）。
  
  android:layout_marginTop：
  30dp：在EditText的顶部与其父布局或上一个视图之间设置30dp的边距。
  
  android:background：
  @drawable/edit_bg：设置EditText的背景为res/drawable目录下的edit_bg资源。
  
  android:drawableStart：
  @drawable/uname：在EditText的文本开始位置绘制一个图标，图标来自res/drawable目录下的uname资源。
  
  android:drawablePadding：
  10dp：设置EditText中的文本与drawableStart图标之间的内边距。
  
  android:hint：
  @string/login_user_hint：为EditText设置一个提示文本，文本内容来自res/values/strings.xml文件中的login_user_hint资源。
  
  android:paddingStart 和 android:paddingEnd：
  30dp：在EditText的文本开始和结束位置设置内边距。

  android:imeOptions：
  actionNext：设置软键盘的“下一步”操作，通常用于表单中的多个输入字段。
  
  android:inputType：
  text：指定EditText接受的输入类型，这里是普通文本。
  
  android:padding：
  5dp：为EditText的内容设置内边距（可能会覆盖paddingStart和paddingEnd的设置，具体取决于Android版本和布局解析器的行为）。
  
  android:importantForAutofill：
  no：指示EditText对于自动填充功能不重要，不应被自动填充服务考虑。

2.快速注释的快捷键：“command + /”，同xcode，但是在xml文件下无法添加注释

3.intent的作用：不同activity之间沟通的载体，即从一个activity跳转至另一个activity时携带的信息通过intent携带；其还有启动activity的作用，消息通知，结果回调的作用，后几个目前没有使用到，后期再进行补充
  intent并非一个实例，而是单独的对象，但也并非所有的activity都会带有一个intent

4.android中的activity的跳转是通过“task”进行堆栈存取的

5.android中的activity类似于ios中的viewController，有几个生命周期，如onCreate()、onStart()、onResume()、onPause()、onStop()、onDestroy()等，后续会补充他们的具体回调时机

