# DIO-desafio-github
Desafio de projeto sobre github 
class Hero {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    atacar() {
        let ataque;
        switch (this.tipo) {
            case "mago":
                ataque = "usou magia";
                break;
            case "guerreiro":
                ataque = "usou espada";
        
                break;
            case "monge":
                ataque = "usou artes marciais";
                break;
            case "ninja":
                ataque = "usou shuriken";
                break;
            default:
                ataque = "usou um ataque indefinido";
        }

        return `o ${this.tipo} atacou usando ${ataque}`;
    }
}

// Exemplo de uso da classe
let heroi = new Hero("Gandalf", 65, "mago");
let mensagem = heroi.atacar();
console.log(mensagem);  // Saída: "o mago atacou usando magia"


