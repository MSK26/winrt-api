---
-api-id: T:Windows.UI.Xaml.Media.Animation.BounceEase
-api-type: winrt class
---

<!-- Class syntax.
public class BounceEase : Windows.UI.Xaml.Media.Animation.EasingFunctionBase, Windows.UI.Xaml.Media.Animation.IBounceEase
-->

# Windows.UI.Xaml.Media.Animation.BounceEase

## -description
Represents an easing function that creates an animated bouncing effect.

## -xaml-syntax
```xaml
<BounceEase .../>
```


## -remarks
[BounceEase](bounceease.md) has two controlling properties [Bounciness](bounceease_bounciness.md) and [Bounces](bounceease_bounces.md) that affect the behavior of the function.

[ElasticEase](elasticease.md) is a similar easing function that works well for physics emulation in animations. The difference with [BounceEase](bounceease.md) is that an [ElasticEase](elasticease.md) can go outside the **From**/**To** range. Another way to conceptualize the two easing functions is that [ElasticEase](elasticease.md) is what you might use to animate the plucking of a string, whereas [BounceEase](bounceease.md) is what you might use to show the bounce of a ball against a line or plane.

An easing function can be applied to the **EasingFunction** properties of **From**/**To**/**By** animations, or to the **EasingFunction** properties of key-frame types used for the **Easing** variants of key-frame animations. For more info, see [Key-frame animations and easing function animations](http://msdn.microsoft.com/library/d8af24cd-f4c2-4562-afd7-25010955d677).

## -examples
The following example applies a [BounceEase](bounceease.md) easing function to a [DoubleAnimation](doubleanimation.md) to create a bouncing effect.



> [!div class="tabbedCodeSnippets"][!code-xml[BounceEase](../windows.ui.xaml.media.animation/code/BounceEase/csharp/Page.xaml#SnippetBounceEase)][!code-vb[BounceEase](../windows.ui.xaml.media.animation/code/BounceEase/vbnet/MainPage.xaml.vb#SnippetBounceEase)]

> [!div class="tabbedCodeSnippets"][!code-cs[BounceEase_code](../windows.ui.xaml.media.animation/code/BounceEase/csharp/Page.xaml.cs#SnippetBounceEase_code)][!code-vb[BounceEase_code](../windows.ui.xaml.media.animation/code/BounceEase/vbnet/MainPage.xaml.vb#SnippetBounceEase_code)]

## -see-also
[Storyboarded animations](http://msdn.microsoft.com/library/0cbceea0-2b0e-44a1-a09a-f7a939632f3a), [Key-frame animations and easing function animations](http://msdn.microsoft.com/library/d8af24cd-f4c2-4562-afd7-25010955d677), [EasingFunctionBase](easingfunctionbase.md), [PowerEase](powerease.md), [BackEase](backease.md), [CircleEase](circleease.md), [CubicEase](cubicease.md), [ElasticEase](elasticease.md), [ExponentialEase](exponentialease.md), [QuadraticEase](quadraticease.md), [QuarticEase](quarticease.md), [QuinticEase](quinticease.md), [SineEase](sineease.md)