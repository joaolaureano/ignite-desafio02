# Middlewares

## Requisitos

[✓] Deve ser possível verificar a existêcia de um usuário em _checksExistsUserAccount_ \
[✓] Deve ser possível verificar se o usuário pode criar um novo _todo_ em _checksCreateTodosUserAvailability_ \
[✓] Deve ser possível verificar se um _todo_ já existe em _checksTodoExists_ \
[✓] Deve ser possível buscar um usuário por _id_ em _findUserById_

---

## Regras de negócio

[✓] _checksExistsUserAccount_ deve agregar user dentro da request caso _username_ exista \
[✓] _checksExistsUserAccount_ não deve passar caso _username_ não exista \
[✓] _checksCreateTodosUserAvailability_ deve permitir a criação de um _todo_ caso o usuário seja _pro_ ou tenha menos de 10 _todos_ já criados \
[✓] _checksCreateTodosUserAvailability_ deve permitir a criação de infinitos _todos_ caso o usuário seja pro \
[✓] _checksCreateTodosUserAvailability_ não deve permitir a criação de um _todo_ caso o usuário não seja pro e tenha 10 ou mais _todos_ já criados \
[✓] _checksTodoExists_ deve agregar _user_ e _todo_ dentro da request caso o _user_ exista e o _todo_ exista e seja associado a ele \
[✓] _checksTodoExists_ não deve passar caso o _id_ do _todo_ não seja associado ao _user_ \
[✓] _checksTodoExists_ não deve passar caso o _id_ não seja do tipo UUID \
[✓] _checksTodoExists_ não deve passar caso o _user_ ou _todo_ não exista \
[✓] _findUserById_ deve agregar o _user_ na requisição caso exista \
[✓] _findUserById_ deve falhar caso o _user_ não exista

<p align="center">
Feito com 💜 por João P. Laureano
</p>
