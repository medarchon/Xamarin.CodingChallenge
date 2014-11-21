In this challenge you'll build a Magic Ball app in Xamarin.Forms and run it on iOS and/or Android.

Xamarin's Developer Center has [Intro to Xamarin.Forms](http://developer.xamarin.com/guides/cross-platform/xamarin-forms/introduction-to-xamarin-forms/) and [XAML](http://developer.xamarin.com/guides/cross-platform/xamarin-forms/xaml-for-xamarin-forms/) docs that will help.

## Challenge

Requirements:
  * Create a new **Xamarin.Forms (PCL)** solution (don't forget to update the NuGet package version to use the latest Xamarin.Forms release)
  * Use XAML to layout your content page.  You'll need at least a textbox, a label, and a button.
  * Allow the user to enter a question
  * Allow the user to ask the question by pressing a button
  * Use the supplied list of Magic 8 ball answers to provide a random answer to the user's question
    
``` 
// http://en.wikipedia.org/wiki/Magic_8-Ball
    " It is certain"
	, " It is decidedly so"
	, " Without a doubt"
	, " Yes definitely"
	, " You may rely on it"
	, " As I see it, yes"
	, " Most likely"
	, " Outlook good"
	, " Yes"
	, " Signs point to yes"
	, " Reply hazy try again"
	, " Ask again later"
	, " Better not tell you now"
	, " Cannot predict now"
	, " Concentrate and ask again"
	, " Don't count on it"
	, " My reply is no"
	, " My sources say no"
	, " Outlook not so good"
	, " Very doubtful "
```

### Bonus Challenge #1

Use the [DependencyService](http://developer.xamarin.com/guides/cross-platform/xamarin-forms/dependency-service/) to read the result using text-to-speech. Sample code for this can be found in the [Todo app](https://github.com/xamarin/xamarin-forms-samples/tree/master/Todo/PCL) (see the [`ITextToSpeech`](https://github.com/xamarin/xamarin-forms-samples/blob/master/Todo/PCL/Todo/ITextToSpeech.cs) interface and its implementations for [iOS](https://github.com/xamarin/xamarin-forms-samples/blob/master/Todo/PCL/Todo.iOS/TextToSpeech_iOS.cs) and [Android](https://github.com/xamarin/xamarin-forms-samples/blob/master/Todo/PCL/Todo.Android/TextToSpeech_Android.cs)).

### Bonus Challenge #2

Use a [CustomRenderer](http://developer.xamarin.com/guides/cross-platform/xamarin-forms/custom-renderer/) to add another button to tweet the result, similar to the `TweetButton` in [this sample](https://github.com/conceptdev/xamarin-forms-samples/blob/master/Evolve13/Evolve13/Controls/TweetButton.cs). It could say something like *"Is my app amazing?"* then append the result.

Don't forget to implement the platform-specific renderers for [iOS](https://github.com/conceptdev/xamarin-forms-samples/blob/master/Evolve13/Evolve13.iOS/TweetButtonRenderer.cs) and [Android](https://github.com/conceptdev/xamarin-forms-samples/blob/master/Evolve13/Evolve13.Android/TweetButtonRenderer.cs).


