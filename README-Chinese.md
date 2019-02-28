![FunnyViews](https://github.com/samlss/FunnyViews/blob/master/logo.png)

## 不积跬步无以至千里

## [English](https://github.com/samlss/FunnyViews/blob/master/README.md)<br>

---

**编程的一部分灵感也来源日常生活<br/><br/>
当我在日常生活中发现一些有趣的view时，我会记录下来并且通过编程实现。<br/><br/>
将记录于android中实现许多有趣的view，包括loadingview，progressview等等，在我创建这些view的时候，没有使用任何图片，我使用Android的原生api来绘制它们。<br/><br/>
如果您有任何有趣的想法，可以联系我729717222@qq.com:cupid:**

---

## 目录

* [时钟类](#%E6%97%B6%E9%92%9F%E7%B1%BB)
  * [ClockView: 一个可爱的时钟](#clockview-%E4%B8%80%E4%B8%AA%E5%8F%AF%E7%88%B1%E7%9A%84%E6%97%B6%E9%92%9F)
* [加载中类](#%E5%8A%A0%E8%BD%BD%E4%B8%AD%E7%B1%BB)
  * [CoffeeView：一杯咖啡的loading view](#coffeeview%E4%B8%80%E6%9D%AF%E5%92%96%E5%95%A1%E7%9A%84loading-view)
  * [FlaskView：一个烧瓶loading view](#flaskview%E4%B8%80%E4%B8%AA%E7%83%A7%E7%93%B6loading-view)
  * [RainyView: 一个下雨view](#rainyview-%E4%B8%80%E4%B8%AA%E4%B8%8B%E9%9B%A8view)
  * [DayNightLoadingView: 一个日夜轮换的loading view](#daynightloadingview-%E4%B8%80%E4%B8%AA%E6%97%A5%E5%A4%9C%E8%BD%AE%E6%8D%A2%E7%9A%84loading-view)
  * [PacmanLoadingView: 一个吃豆豆的loading view](#pacmanloadingview-%E4%B8%80%E4%B8%AA%E5%90%83%E8%B1%86%E8%B1%86%E7%9A%84loading-view)
  * [PinBallLoadingView: 一个弹球球loading view](#pinballloadingview-%E4%B8%80%E4%B8%AA%E5%BC%B9%E7%90%83%E7%90%83loading-view)
  * [PeasLoadingView: 一个小豆豆旋转loading view](#peasloadingview-%E4%B8%80%E4%B8%AA%E5%B0%8F%E8%B1%86%E8%B1%86%E6%97%8B%E8%BD%ACloading-view)
  * [ClockLoadingView: 一个时钟loading view](#clockloadingview-%E4%B8%80%E4%B8%AA%E6%97%B6%E9%92%9Floading-view)
  * [SignalLoadingView: 一个信号旋转loading view](#signalloadingview-%E4%B8%80%E4%B8%AA%E4%BF%A1%E5%8F%B7%E6%97%8B%E8%BD%ACloading-view)
  * [JumboLoadingView: 一个可以选择形状并且可设置进度的view](#jumboloadingview-%E4%B8%80%E4%B8%AA%E5%8F%AF%E4%BB%A5%E9%80%89%E6%8B%A9%E5%BD%A2%E7%8A%B6%E5%B9%B6%E4%B8%94%E5%8F%AF%E8%AE%BE%E7%BD%AE%E8%BF%9B%E5%BA%A6%E7%9A%84view)
  * [FanLoadingView: 一个风扇旋转的loading view](#fanloadingview-%E4%B8%80%E4%B8%AA%E9%A3%8E%E6%89%87%E6%97%8B%E8%BD%AC%E7%9A%84loading-view)
  * [WhirlLoadingView: 一个包含两条圆弧互相旋转的loading view](#whirlloadingview-%E4%B8%80%E4%B8%AA%E5%8C%85%E5%90%AB%E4%B8%A4%E6%9D%A1%E5%9C%86%E5%BC%A7%E4%BA%92%E7%9B%B8%E6%97%8B%E8%BD%AC%E7%9A%84loading-view)
  * [CubeLoadingView:一个立体3D旋转的loading view](#cubeloadingview%E4%B8%80%E4%B8%AA%E7%AB%8B%E4%BD%933d%E6%97%8B%E8%BD%AC%E7%9A%84loading-view)
  * [DiceLoadingView:一个骰子3D旋转loading view](#diceloadingview%E4%B8%80%E4%B8%AA%E9%AA%B0%E5%AD%903d%E6%97%8B%E8%BD%ACloading-view)
  * [BarChartLoadingView:一个可以指定条形数量的条形图loading view](#barchartloadingview%E4%B8%80%E4%B8%AA%E5%8F%AF%E4%BB%A5%E6%8C%87%E5%AE%9A%E6%9D%A1%E5%BD%A2%E6%95%B0%E9%87%8F%E7%9A%84%E6%9D%A1%E5%BD%A2%E5%9B%BEloading-view)
  * [BallsLoadingView：一个包含四个做循环动画的小球的loading view](#ballsloadingview%E4%B8%80%E4%B8%AA%E5%8C%85%E5%90%AB%E5%9B%9B%E4%B8%AA%E5%81%9A%E5%BE%AA%E7%8E%AF%E5%8A%A8%E7%94%BB%E7%9A%84%E5%B0%8F%E7%90%83%E7%9A%84loading-view)
  * [IntertwineLoadingView：两个交织的小球的loading view](#intertwineloadingview%E4%B8%A4%E4%B8%AA%E4%BA%A4%E7%BB%87%E7%9A%84%E5%B0%8F%E7%90%83%E7%9A%84loading-view)
* [进度类](#%E8%BF%9B%E5%BA%A6%E7%B1%BB)
  * [JumboLoadingView: 一个可以选择形状并且可设置进度的view](#jumboloadingview-%E4%B8%80%E4%B8%AA%E5%8F%AF%E4%BB%A5%E9%80%89%E6%8B%A9%E5%BD%A2%E7%8A%B6%E5%B9%B6%E4%B8%94%E5%8F%AF%E8%AE%BE%E7%BD%AE%E8%BF%9B%E5%BA%A6%E7%9A%84view-1)
  * [DonutProgressView: 一个简洁的进度view](#donutprogressview-%E4%B8%80%E4%B8%AA%E7%AE%80%E6%B4%81%E7%9A%84%E8%BF%9B%E5%BA%A6view)
  * [CircleProgressView:一个简约的圆圈进度view](#circleprogressview%E4%B8%80%E4%B8%AA%E7%AE%80%E7%BA%A6%E7%9A%84%E5%9C%86%E5%9C%88%E8%BF%9B%E5%BA%A6view)
* [充电类](#%E5%85%85%E7%94%B5%E7%B1%BB)
  * [ChargingView: 一个简单的充电view](#chargingview-%E4%B8%80%E4%B8%AA%E7%AE%80%E5%8D%95%E7%9A%84%E5%85%85%E7%94%B5view)
  * [PowerView: 一个简约的充电view](#powerview-%E4%B8%80%E4%B8%AA%E7%AE%80%E7%BA%A6%E7%9A%84%E5%85%85%E7%94%B5view)
* [其他](#%E5%85%B6%E4%BB%96)
  * [Bling: 图形下落效果](#bling-%E5%9B%BE%E5%BD%A2%E4%B8%8B%E8%90%BD%E6%95%88%E6%9E%9C)
* [使用说明](#%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E)
* [License](#license)


---

# 时钟类
## [ClockView: 一个可爱的时钟](https://github.com/samlss/ClockView)<br>
![ClcokView](https://github.com/samlss/ClockView/blob/master/screenshots/screenshot1.gif)
<br>
![ClcokView](https://github.com/samlss/ClockView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>



# 加载中类
## [CoffeeView：一杯咖啡的loading view](https://github.com/samlss/CoffeeView)<br>
![CoffeeView](https://github.com/samlss/CoffeeView/blob/master/screenshots/screenshot1.gif)<br>
![CoffeeView](https://github.com/samlss/CoffeeView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

## [FlaskView：一个烧瓶loading view](https://github.com/samlss/FlaskView)<br>
![FlaskView](https://github.com/samlss/FlaskView/blob/master/screenshots/screenshot1.gif)<br>
![FlaskView](https://github.com/samlss/FlaskView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

## [RainyView: 一个下雨view](https://github.com/samlss/RainyView)<br>
![RainyView](https://github.com/samlss/RainyView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [DayNightLoadingView: 一个日夜轮换的loading view](https://github.com/samlss/DayNightLoadingView)<br>
![DayNightLoadingView](https://github.com/samlss/DayNightLoadingView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [PacmanLoadingView: 一个吃豆豆的loading view](https://github.com/samlss/PacmanLoadingView)<br>
![PacmanLoadingView](https://github.com/samlss/PacmanLoadingView/blob/master/screenshots/screenshot4.gif)
<br>
<br>
<br>

## [PinBallLoadingView: 一个弹球球loading view](https://github.com/samlss/PinBallLoadingView)<br>
![PinBallLoadingView](https://github.com/samlss/PinBallLoadingView/blob/master/screenshots/screenshot1.gif)

![PinBallLoadingView](https://github.com/samlss/PinBallLoadingView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

## [PeasLoadingView: 一个小豆豆旋转loading view](https://github.com/samlss/PeasLoadingView)<br>
![PeasLoadingView](https://github.com/samlss/PeasLoadingView/blob/master/screenshots/screenshot3.gif)
<br>
<br>
<br>

## [ClockLoadingView: 一个时钟loading view](https://github.com/samlss/ClockLoadingView)<br>
![ClockLoadingView](https://github.com/samlss/ClockLoadingView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [SignalLoadingView: 一个信号旋转loading view](https://github.com/samlss/SignalLoadingView)<br>
![ClockLoadingView](https://github.com/samlss/SignalLoadingView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [JumboLoadingView: 一个可以选择形状并且可设置进度的view](https://github.com/samlss/JumboLoadingView)<br>
![screenshot_circle](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_circle.gif)
![screenshot_square](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_square.gif)
![screenshot_triangel](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_triangel.gif)
![screenshot_star](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_star.gif)
<br>
<br>
<br>

## [FanLoadingView: 一个风扇旋转的loading view](https://github.com/samlss/FanLoadingView)<br>
![FanLoadingView](https://github.com/samlss/FanLoadingView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [WhirlLoadingView: 一个包含两条圆弧互相旋转的loading view](https://github.com/samlss/WhirlLoadingView)<br>
![WhirlLoadingView](https://github.com/samlss/WhirlLoadingView/blob/master/screenshots/screenshot.gif)
<br>
<br>
<br>

## [CubeLoadingView:一个立体3D旋转的loading view](https://github.com/samlss/CubeLoadingView)<br>
![WhirlLoadingView](https://github.com/samlss/CubeLoadingView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [DiceLoadingView:一个骰子3D旋转loading view](https://github.com/samlss/DiceLoadingView)<br>
![DiceLoadingView](https://github.com/samlss/DiceLoadingView/blob/master/screenshots/screenshot1.gif)<br>
![DiceLoadingView](https://github.com/samlss/DiceLoadingView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

## [BarChartLoadingView:一个可以指定条形数量的条形图loading view](https://github.com/samlss/BarChartLoadingView)<br>
![BarChartLoadingView](https://github.com/samlss/BarChartLoadingView/blob/master/screenshots/screenshot1.gif)<br>
![BarChartLoadingView](https://github.com/samlss/BarChartLoadingView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

## [BallsLoadingView：一个包含四个做循环动画的小球的loading view](https://github.com/samlss/BallsLoadingView)<br>
![BallsLoadingView](https://github.com/samlss/BallsLoadingView/blob/master/screenshots/screenshot1.gif)<br>
![BallsLoadingView](https://github.com/samlss/BallsLoadingView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

## [IntertwineLoadingView：两个交织的小球的loading view](https://github.com/samlss/IntertwineLoadingView)<br>
![IntertwineLoadingView](https://github.com/samlss/IntertwineLoadingView/blob/master/screenshots/screenshot1.gif)
<br>
<br>

# 进度类
## [JumboLoadingView: 一个可以选择形状并且可设置进度的view](https://github.com/samlss/JumboLoadingView)<br>
![screenshot_circle](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_circle.gif)
![screenshot_square](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_square.gif)
![screenshot_triangel](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_triangel.gif)
![screenshot_star](https://github.com/samlss/JumboLoadingView/blob/master/screenshots/screenshot_star.gif)
<br>
<br>
<br>

## [DonutProgressView: 一个简洁的进度view](https://github.com/samlss/DonutProgressView)<br>
![DonutProgressView](https://github.com/samlss/DonutProgressView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

## [CircleProgressView:一个简约的圆圈进度view](https://github.com/samlss/CircleProgressView)<br>
![CircleProgressView](https://github.com/samlss/CircleProgressView/blob/master/screenshots/screenshot1.gif)
<br>
<br>
<br>

# 充电类
## [ChargingView: 一个简单的充电view](https://github.com/samlss/ChargingView)<br>
![ChargingView](https://github.com/samlss/ChargingView/blob/master/screenshot/screenshot1.gif)
<br>
<br>
<br>

## [PowerView: 一个简约的充电view](https://github.com/samlss/PowerView)<br>
![PowerView](https://github.com/samlss/PowerView/blob/master/screenshots/screenshot1.gif)<br/>
![PowerView](https://github.com/samlss/PowerView/blob/master/screenshots/screenshot2.gif)
<br>
<br>
<br>

# 其他
## [Bling: 图形下落效果](https://github.com/samlss/Bling)<br>
![Bling](https://github.com/samlss/Bling/blob/master/screenshots/screenshot5.gif)
<br>
<br>
<br>


# 使用说明
#### 当你使用其中一个项目的时候, star和反馈是对我开发的认可和支持，谢谢

# License
#### 每个的项目都有对应的license，你可以进入某一个项目进行查看

