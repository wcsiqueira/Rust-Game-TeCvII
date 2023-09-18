# JOGO DA COBRINHA
 Jogo feito na disciplina TECVII- Universidade federal de Pelotas 
Baseado no exemplo encontrado na biblioteca ggezÇhttps://github.com/ggez/ggez

REFERENCIAS 
https://rust-br.github.i
https://www.youtube.com/watch?v=DnT_7M7L7vo&t=464s
https://www.youtube.com/watch?v=iR7Q_6quwSI&t=2172s
https://www.youtube.com/watch?v=AYfehnFklkA
https://www.youtube.com/watch?v=8DUENLiOfiQ&t=1868s

Não esquecer de usar a biblioteza GGEZ [ggez](https://crates.io/crates/ggez)

## Requer
1. Precisa instalar o RUST [installed](https://www.rust-lang.org/en-US/install.html)
2.iNSTALE EM SEU CARGO.TOML [SDL2 libraries](https://github.com/Rust-SDL2/rust-sdl2#requirements)

### Use cargo run no dicionário do projeto para rodar o jogo

````
```

//fn main() -> GameResult {
    // Primeiro, criamos uma estrutura `ggez::Conf` que define as configurações do nosso jogo.
    let (ctx, event_loop) = ggez::ContextBuilder::new("Jogo da Cobrinha-=TECVII", "welder")
        // Primeiro, criamos uma estrutura `ggez::Conf` que define as configurações do nosso jogo.
        .window_setup(ggez::conf::WindowSetup::default().title("Jogo da Cobrinha!!!"))
       // Em seguida, chamamos a função `ggez::ContextBuilder::new` para criar um `ContextBuilder`,
    // que nos permitirá personalizar como queremos que o contexto seja criado.
        .window_mode(
            ggez::conf::WindowMode::default()
                .dimensions(SCREEN_SIZE.0 as f32, SCREEN_SIZE.1 as f32),
        )
        
        // CASO DE ERRADO, VAI DAR RUIM!!!!!!
        .build()
        .expect("DEU RUIM!!!!!!");
   // Em seguida, criamos uma instância do nosso `GameState` e a passamos para a função
    // `ggez::event::run` para iniciar o loop principal do jogo.
    let state = GameState::new()?;
   
    event::run(ctx, event_loop, state)
}



```
````
![game_INICIOt](resources/Cobrinha.png)

