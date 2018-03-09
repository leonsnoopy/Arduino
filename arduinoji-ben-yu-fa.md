# 基本語法

```Arduino
void setup() //初始設定區塊 (只執行一次)
{
 pinMode(ledPin, OUTPUT); //設定pin腳模式為輸出
}
void loop() //重複執行區塊 (不斷地重複執行)
{
 digitalWrite(ledPin, HIGH); //給pin腳高電壓 (LED通電就亮)
 delay(1000); //延遲1秒鐘(1000毫秒)                 
 digitalWrite(ledPin, LOW);     //給pin腳低電壓 (LED不通電就暗)
 delay(1000); //延遲1秒鐘(1000毫秒)
}
```

setup  可以設定 pin 為 輸出/輸入作用

HIGH 跟 LOW 參數為是否有通電

