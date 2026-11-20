# Presets

Each `.txt` file here is one workout. It shows up as a button under "Start from" on the setup screen.

## Adding a preset

1. Create a new `.txt` file in this folder, for example `tempo-25.txt`.
2. Add its file name to `presets.json`. Buttons appear in the order the files are listed.

## File format

The format is the same as the "Workout script" box on the setup screen:

```
# Tempo 25
5:00, 80, 30, Warm-up
15:00, 90-95, 42, Tempo
5:00, 75, 25, Cool-down
```

- The first line, `# Name`, is the button label. Without it, the file name is used instead.
- Each line after that is one segment: time, cadence (rpm), resistance (0 to 100), label.
- Cadence and resistance can be ranges, such as `85-95`.
- Any other line starting with `#` is ignored, so you can use them for notes.
