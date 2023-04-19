# Redmi-2--mobian12


fastboot模式一键刷入


骁龙410
主线6.2内核
主频1Ghz
只有摄像不工作和没声音

果你的手机在插卡之后检测到卡但是没有信号，则你的手机型号是wt86047。
使用和wt88047不一样的modem固件。
可以通过adb来切换modem固件解决。
adb shell
cp lib/firmware-wt86047/* lib/firmware/

某些红米2的屏幕驱动暂时不能正确处理屏幕休眠，休眠唤醒之后可能会有轻微的残影或者闪屏现象
已知完美的屏幕有 mdss_dsi_nt35521_720p_video 不会闪屏和残影。
屏幕型号请参见lk2nd的PANEL那一栏.
