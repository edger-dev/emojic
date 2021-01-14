# emojic 😀 🙂 😇
Emoji constants for your rusty strings. This crate is rustlang port of [emoji](https://github.com/enescakir/emoji) written by [@enescakir](https://github.com/enescakir)

![License](https://img.shields.io/github/license/orhanbalci/emojic.svg)


# 📦 Cargo.toml
```
emojic = {git = "https://github.com/orhanbalci/emojic.git"}
```
# 🔧 Example
```rust
use emojic::constants::*;

fn main() {
    println!("Hello {}", WAVING_HAND);
    println!(
        "I'm {} from {}",
        MAN_TECHNOLOGIST,
        FLAG_TURKEY
    );
    println!(
        "Different skin tones default {} light {} dark {}",
        THUMBS_UP,
        OK_HAND.tone(vec![Tone::LIGHT]),
        CALL_ME_HAND.tone(vec![Tone::DARK])
    );
    println!(
        "Emojis with multiple skin tones.\nBoth medium: {} light and dark: {}",
        PEOPLE_HOLDING_HANDS.tone(vec![Tone::MEDIUM]),
        PEOPLE_HOLDING_HANDS.tone(vec![Tone::LIGHT, Tone::DARK])
    );
}

```
# 🖨️ Output
```
Hello 👋
I'm 👨‍💻 from 🇹🇷
Different skin tones default 👍 light 👌🏻 dark 🤙🏿
Emojis with multiple skin tones.
Both medium: 🧑🏽‍🤝‍🧑🏽 light and dark: 🧑🏻‍🤝‍🧑🏿
```
