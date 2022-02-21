<a href="https://pub.dev/packages/confirmation_slider"><img src="https://img.shields.io/pub/v/confirmation_slider.svg?style=flat?logo=dart" alt="pub.dev"></a>
<a href="https://github.com/SplashByte/confirmation_slider"><img src="https://img.shields.io/static/v1?label=platform&message=flutter&color=1ebbfd" alt="github"></a>
[![likes](https://badges.bar/confirmation_slider/likes)](https://pub.dev/packages/confirmation_slider/score)
[![popularity](https://badges.bar/confirmation_slider/popularity)](https://pub.dev/packages/confirmation_slider/score)
[![pub points](https://badges.bar/confirmation_slider/pub%20points)](https://pub.dev/packages/confirmation_slider/score)
<a href="https://github.com/SplashByte/confirmation_slider/blob/main/LICENSE"><img src="https://img.shields.io/github/license/SplashByte/confirmation_slider.svg" alt="license"></a>

[![buy me a coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/splashbyte)

### If you like this package, please leave a like there on [pub.dev](https://pub.dev/packages/confirmation_slider) and star on [GitHub](https://github.com/SplashByte/confirmation_slider).

A slider to confirm actions and provide feedback on the success of these after subsequent loading.

## Examples

![confirmation_slider](https://user-images.githubusercontent.com/43761463/147601537-a09d9772-abfa-4409-88c7-1f1e0f04c27a.gif)
![confirmation_slider_rolling](https://user-images.githubusercontent.com/43761463/147601547-ae8200b0-668c-4d1d-a7e5-80691e156a62.gif)
![confirmation_slider_custom](https://user-images.githubusercontent.com/43761463/147602062-87f55f38-9cbf-4a89-ae4d-48ca81317dca.gif)

## Easy Usage

Easy to use and highly customizable.

```dart
ConfirmationSlider.standard(
    width: 300.0,
    child: const Text('Slide to confirm'),
    successIcon: const Icon(Icons.check_rounded, color: Colors.white),
    onSlide: (loading, success, failure) async {
        loading(); //or controller.loading()
        await Future.delayed(const Duration(seconds: 3));
        success(); //or controller.success()
    },
),
```