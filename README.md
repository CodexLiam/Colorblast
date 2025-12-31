# ColorBlast

**ColorBlast** is a Python library for colorful, animated, and highly stylized console output. It enhances terminal scripts, CLI apps, or games with text effects, emojis, and animations.

---

## Installation

```bash
pip install colorblast
````

---

## Features

ColorBlast provides a wide variety of console effects:

### 1. Basic Printing

Print colored and styled text with optional typing effect and emoji:

```python
from colorblast import ColorBlast

ColorBlast.print("Hello World!", color="cyan", style="bold", typing_speed=0.05, emoji="star")
```

**Parameters:**

* `color`: red, green, yellow, blue, magenta, cyan, white
* `style`: bold, italic, underline, blink, reverse
* `typing_speed`: delay per character (seconds)
* `emoji`: emojis such as star, fire, info, success

---

### 2. Gradient Text

Display text with smooth color gradients:

```python
ColorBlast.print("Gradient Magic!", gradient=True, typing_speed=0.03)
```

---

### 3. Frames / Boxes

Draw multi-line frames with custom border character, color, and style:

```python
ColorBlast.framed("Multi-line frame\nWith colors", border_char="#", color="magenta", style="underline")
```

---

### 4. Log-Level Messages

Convenient logging with emojis and colors:

```python
ColorBlast.log("This is an info message", level="INFO")
ColorBlast.log("Warning! Something went wrong", level="WARNING")
ColorBlast.log("Error occurred!", level="ERROR")
ColorBlast.log("Success! Task completed", level="SUCCESS")
```

---

### 5. Animations

**Letter Scramble Animation**

```python
ColorBlast.animated("Loading...", duration=3, color="cyan", style="bold")
```

**Confetti**

```python
ColorBlast.confetti("Party Time!", duration=3)
```

**Fireworks**

```python
ColorBlast.fireworks("Boom! 🎆", duration=3)
```

---

### 6. Scrolling / Marquee Text

```python
ColorBlast.marquee("Scrolling text demo", width=50, speed=0.1, repeat=2)
```

---

### 7. Countdown Timer

```python
ColorBlast.countdown(5, color="yellow", style="bold")
```

---

### 8. Sparkle Effect

```python
ColorBlast.sparkle("Sparkle Magic!", duration=3)
```

---

### 9. Rainbow Text

```python
ColorBlast.rainbow("Rainbow Text!", speed=0.05, repeat=1)
```

---

### 10. Progress Bar

```python
ColorBlast.progress_bar(total=20, duration=5, color="green")
```

---

### 11. Advanced Styles

Combine options for blinking or inverted text:

```python
ColorBlast.print("Blinking Text!", blink=True, color="red")
ColorBlast.print("Inverted Text!", reverse=True, color="cyan")
```

---

## Full Example

```python
from colorblast import ColorBlast

# Basic print with emoji
ColorBlast.print("Hello World!", color="cyan", style="bold", typing_speed=0.05, emoji="star")

# Framed multi-line text
ColorBlast.framed("Multi-line frame\nWith colors", border_char="#", color="magenta", style="underline")

# Log levels
ColorBlast.log("Loading complete!", level="SUCCESS")

# Animations
ColorBlast.animated("Processing...", duration=3, color="blue", style="bold")
ColorBlast.confetti("Party Time!", duration=3)
ColorBlast.fireworks("Boom! 🎆", duration=3)

# Scrolling text
ColorBlast.marquee("Scrolling Text Demo", width=50, speed=0.1, repeat=2)

# Countdown
ColorBlast.countdown(5, color="yellow", style="bold")

# Sparkle effect
ColorBlast.sparkle("Sparkle Magic!", duration=3)

# Rainbow text
ColorBlast.rainbow("Rainbow Text!", speed=0.05, repeat=1)

# Progress bar
ColorBlast.progress_bar(total=20, duration=5, color="green")
```
