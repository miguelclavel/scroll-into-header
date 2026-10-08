# Scroll Into Header

A name that travels into the header, from [miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=scroll-into-header).

<img src="assets/demo.gif" width="720" alt="A name that travels into the header: a screen recording">

**[Try it live](https://miguelclavel.github.io/scroll-into-header/)** · one file, `index.html`, no libraries, no build step.

My name starts in the middle of the screen and ends up in the header.

It doesn't fade out and reappear up there. It actually travels.

Most portfolios have a big name on the first screen and a small one in the bar at the top, and they're two separate things. Swap one for the other and the reader feels the cut. I wanted one object that moves, so you always know where the name went.

Here's the whole idea in four steps.

1. Make the hero section tall, a few screens worth, and pin what's inside it to the top of the viewport while you scroll through.

2. Turn scroll position into one number between 0 and 1. How far are we through this tall section. That's the only input.

3. Feed that number into everything at once. The size of the name, where it sits, how much the rest fades. Nothing gets its own timer.

4. Bend the number through an easing curve before you use it. Straight lines feel mechanical. It's the step people skip and it's the one you actually feel.

The nice part is you can tune it forever by changing one number.

## Use it on your site

Put your name in the fixed `.name` heading and an invisible copy of it in the header (`.slot`), which is where it parks. Wrap the first screen in the tall `.track` with a sticky `.stage` inside, and copy the script from `index.html`. Make the track taller for a slower journey, or swap `easeOut` for another curve. For people who prefer reduced motion it jumps straight to the header.

## Or build your own from the prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Make my hero section three screens tall and pin its contents to the top while the user scrolls through it. Turn the scroll position inside that section into a single value from 0 to 1. Use that one value to move my name from large and centered to small and top left, and to fade the supporting text out as it goes. Run the value through an ease-out curve before applying it. When the section ends, leave the name parked in the header for the rest of the page.
```

More like this in [interaction-recipes](https://github.com/miguelclavel/interaction-recipes).

---

MIT licensed. Made by [Miguel Clavel](https://miguelclavel.com/?utm_source=github&utm_medium=scroll-into-header) with Claude Code. If you build one of these, send it to me. I'd genuinely like to see it.
