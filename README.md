# Validador de CNPJ e CPF

Este é um script/programa Python multiplataforma (Windows/Linux/Mac) para validação e cálculo dos dígitos verificadores de CNPJs e CPFs.

---

## Como usar

*Obs: É preciso ter o Python instalado, você pode baixá-lo [aqui](https://www.python.org/downloads/).*

Após baixar o arquivo .py (se não baixou ainda, pode baixá-lo [aqui](https://github.com/eduardoranucci/validador-cnpj-cpf/releases)), abra um terminal na mesma pasta onde o arquivo foi baixado.

---

### Validar os dígitos verificadores do CNPJ

Para validar um CNPJ, digite esse comando:

`> python validador.py -cnpj <CNPJ>`

Ex1:

`> python validador.py -cnpj 18781203000128`

Ou

`> python validador.py -cnpj 18.781.203/0001-28`

Nos dois caso o resultado será o mesmo:

`Output: Os dígitos verificadores estão corretos.`

Ex2:

`> python validador.py -cnpj 18.781.203/0001-69`

```
Output: 

Os dígitos verificadores estão incorretos.

CNPJ: 18.781.203/0001-28

```

---

### Calcular dígitos verificadores do CNPJ

Caso não saiba os dígitos verificadores, você pode digitar o CNPJ sem eles e o programa calculará para você.

Ex:

`> python validador.py -cnpj 187812030001`

Ou

`> python validador.py -cnpj 18.781.203/0001`

Nos dois caso o resultado será o mesmo:

`Output: CNPJ: 18.781.203/0001-28`


---

### Validar os dígitos verificadores do CPF

Para validar um CPF, digite esse comando:

`> python validador.py -cpf <CPF>`

Ex1:

`> python validador.py -cpf 28001238938`

Ou

`> python validador.py -cpf 280.012.389-38`

Nos dois caso o resultado será o mesmo:

`Output: Os dígitos verificadores estão corretos.`

Ex2:

`> python validador.py -cpf 280.012.389-24`

```
Output: 

Os dígitos verificadores estão incorretos.

CPF: 280.012.389-38

```

---

### Calcular dígitos verificadores do CPF

Caso não saiba os dígitos verificadores, você pode digitar o CPF sem eles e o programa calculará para você.

Ex:

`> python validador.py -cpf 280012389`

Ou

`> python validador.py -cpf 280.012.389`

Nos dois caso o resultado será o mesmo:

`Output: CPF: 280.012.389-38`


---

LICENSE

MIT License

Copyright (c) 2022 Eduardo Ranucci

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.