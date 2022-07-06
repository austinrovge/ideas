# beeg-app

There are countless times when I'm lifting and I want to double check:
1. What the proper form is
2. What exact muscle this exercise is working
3. What exercise I should do to target a specific muscle
4. Visual indicator of eccentric/concentric/pause at peak of rep
    * Apple Watch integration 👀
6. What my last PR was for an exercise (journaling)
7. AI/manually saved "playlists" of exercises to do with sets/reps for each
8. Record my form and see how straight my body moves the bar

This is pretty similar to [MuscleWiki](https://apps.apple.com/us/app/musclewiki-fitness/id1096827640). I downloaded this app years ago but haven't ever used it. Actually, opening it again while writing this shows that it addresses #1 (indirectly), #2 (kinda), and #3. It even has a cool calorie, macro, and one rep max calulator in it!

However, it feels sluggish when scrolling through the list of exercises for a muscle as the infinite scroll loads more exercises. Searching for an exercise (#2) takes me to a web page (using `SFSafariViewController`) with a list of results which feels clunky. I'd like to see more tips/tricks around form (#1) and even more from it. That makes it perfect to work on!

#7 is similar to [Iron Path](https://apps.apple.com/us/app/iron-path/id955364910). However this app doesn't seem like it's been updated in some time. The app renders in a smaller phone size that isn't native to iPhone 12 Pro Max. A "Shake to send Feedback" box appears as well! Haven't seen that in a while.

### Scope

The bullets are conveiniently in order of how hard the requirement is:
* #1 through #3 are hard requirements for this. That is the bare minimum to replicate the functionality already mostly available from MuscleWiki.
* #4 would be a **fantastic** feature! I would love this. I try my best to remember timings, but I'm not great at remembering to remember it.
* #5 I think would be very useful, though it's not something I'm dying for today - I could get by with writing this into the system Notes app but I don't.
* #6 would be neat. Maybe being able to "randomize" a playlist so it swaps out exercises with other exercises that work the same muscle group(s). Keep the body alert instead of always doing the same old same old.
* #7 would be pretty cool to implement but I don't think I would use it frequently. Maybe in the future when lifting heavier weights.

### Technologies

* SwiftUI
* Jetpack compose
  * If I don't go with a 17-in-1 framework, I don't think I'll port it to another platform 😬
* PWA (JavaScript probably 🤢)
* React Native 🤢
* Flutter 🤢
* Xamarin/MAUI 🤢
