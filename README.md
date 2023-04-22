# Mandelbrot

## Run the application

```
cargo run mandel.png 1000x800 -1.20,0.35 -1,0.20
```

![Example output](mandel.png)

## Release build

```
cargo build --release
```

### Running time on single core

```
time target/release/mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20

target/release/mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
3.53s  user
0.01s  system
89%    cpu
3.951  total
```

### Running time on 8 threads

```
❯ time target/release/mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
target/release/mandelbrot mandel.png 4000x3000 -1.20,0.35 -1,0.20
3.82s user
0.01s system
257% cpu
1.487 total
```
