# Examples

## Basic Conversions

```clojure
(use Color)

(defn main []
  (let [c (Color.red)
        h (Color.rgb-to-hsl &c)
        light (Color.lighten &c 0.2)
        hex (Color.to-hex &light)]
    (println* "Hex: " hex)))
```

## Parsing Hex

```clojure
(match (Color.from-hex "#3498db")
  (Result.Success c) (println* "HSL: " (str &(Color.rgb-to-hsl &c)))
  (Result.Error msg) (println* "Error: " msg))
```

## Mixing Colors (Lerp)

```clojure
(let [c1 (Color.red)
      c2 (Color.blue)
      mid (Color.lerp &c1 &c2 0.5)]
  (println* "Mid: " (str &mid)))
```
