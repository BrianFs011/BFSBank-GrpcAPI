# BFSBank — gRPC API (.NET 11)

Parte integrante do ecossistema multi-repo **BFSBank**, explorando o paradigma de **gRPC sobre HTTP/2** e serialização binária com **Protocol Buffers (Protobuf)** para comunicação inter-serviços de altíssima performance e baixa latência dentro da malha de microsserviços do banco.

---

## 🚀 Como Executar

### Pré-requisitos
* [.NET 11 SDK](https://dotnet.microsoft.com/download)

### 1. Confiar no certificado HTTPS de desenvolvimento (se ainda não feito)
```bash
dotnet dev-certs https --trust
```

### 2. Rodar a aplicação com perfil HTTPS
```bash
dotnet run --launch-profile https
```

* **URL gRPC (HTTP/2):** `https://localhost:7196`
* **Contrato Protobuf:** [Protos/greet.proto](./Protos/greet.proto)

---

## 🏛️ Características do Paradigma
* **HTTP/2 Multiplexing**: Canal persistente com tráfego bidirecional e cabeçalhos compactados (HPACK).
* **Protobuf**: Serialização binária fortemente tipada, ideal para mensageria interna e transações de liquidação entre nós do cluster.

---

Desenvolvido por [Brian Ferreira da Silva](https://github.com/BrianFs011) — Portfólio de Engenharia.
