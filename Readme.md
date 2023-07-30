## Instrucciones para instalar Rust usando entornos conda

### Paso 1: Instalar Rust

1. Abre una terminal, ubicate en el directorio que quieras instalar Rust y ejecuta el siguiente comando para crear un entorno conda para Rust en la ubicación e instalar Rust en el entorno:

```
conda create -p .env_rust -c conda-forge rust
```

### Paso 2: Activar el entorno Rust

1. Abre una terminal y ejecuta el siguiente comando para activar el entorno Rust:

```
conda activate ./.env_rust
```

### Paso 3: Verificar la instalación

1. Abre una terminal y ejecuta el siguiente comando para verificar la instalación de Rust:

```
rustc --version
```

Debería ver una salida similar a la siguiente:

```
rustc 1.71.0 (8ede3aae2 2023-07-12)
```

### Paso 4: ¡Ahora estás listo para comenzar a codificar en Rust!

## Código de ejemplo 1: ¡Hola mundo!

Aquí hay un pequeño código de ejemplo que muestra cómo usar Rust para imprimir "Hola mundo!" en la consola:

```
fn main() {
  println!("¡Hola mundo!");
}
```

Para compilar y ejecutar este código, abre una terminal en el directorio que contiene el código y ejecuta los siguientes comandos:

```
rustc hello_world.rs
./hello_world
```

¡Deberías ver la siguiente salida en la consola:

```
¡Hola mundo!
```

## Código de ejemplo 2: ¡Hola mundo! (con Cargo)

Let's write a small application with our new Rust development environment. To start, we'll use Cargo to make a new project for us. In your terminal of choice run:

```
cargo new hello-rust
```

This will generate a new directory called hello-rust with the following files:

```
hello-rust
|- Cargo.toml
|- src
  |- main.rs
```

Cargo.toml is the manifest file for Rust. It's where you keep metadata for your project, as well as dependencies.

src/main.rs is where we'll write our application code.

cargo new generates a "Hello, world!" project for us! We can run this program by moving into the new directory that we made and running this in our terminal:

```
cd hello-rust
cargo run
```

You should see this in your terminal:

```
$ cargo run
Compiling hello-rust v0.1.0 (/Users/ag_dubs/rust/hello-rust)
Finished dev [unoptimized + debuginfo] target(s) in 1.34s
Running `target/debug/hello-rust`
Hello, world!
```

### Nota: Es posible que necesites instalar un compilador C

Es posible que necesites instalar las herramientas de compilación de Visual Studio C++ cuando se te solicite hacerlo. Si no estás en Windows, consulta "Otros métodos de instalación".

## Visual Studio C++ Build tools:

https://visualstudio.microsoft.com/visual-cpp-build-tools/

## Otros métodos de instalación

https://forge.rust-lang.org/infra/other-installation-methods.html
