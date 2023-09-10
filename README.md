# devops-netology

<<<<<<< HEAD
# 05-virt-02-iaac
=======
# 05-virt-02-basics
>>>>>>> refs/remotes/origin/master

## Задача 1
_Опишите основные преимущества применения на практике IaaC-паттернов._

Ответ:

IaaS (Infrastructure as a Service) — это модель облачных вычислений, которая предоставляет виртуальные вычислительные ресурсы через интернет. Паттерны IaaS (или IaaC - Infrastructure as Code) - это методология управления инфраструктурой с использованием кода. Применение IaaC-паттернов на практике имеет множество преимуществ:

1. **Автоматизация и консистентность**: IaaC позволяет создавать и управлять инфраструктурой с помощью кода, что обеспечивает автоматизацию процессов. Это снижает вероятность человеческих ошибок и обеспечивает консистентность в развертывании и управлении ресурсами.

2. **Скорость и гибкость**: IaaC позволяет масштабировать и изменять инфраструктуру с минимальными усилиями. Вы можете быстро создавать, изменять и уничтожать ресурсы в зависимости от потребностей вашего приложения или бизнес-проекта.

3. **Повторяемость**: Вы можете легко воссоздавать всю инфраструктуру с помощью кода. Это особенно полезно в случае отказа или необходимости развертывания среды в другом регионе.

4. **Масштабируемость**: IaaC позволяет легко масштабировать вашу инфраструктуру вверх или вниз в зависимости от нагрузки. Можно создавать шаблоны, которые автоматически увеличивают ресурсы при необходимости.

5. **Управление версиями**: Код инфраструктуры может быть управляем с использованием систем контроля версий (например, Git). Это обеспечивает отслеживание изменений и управление версиями  инфраструктуры, что упрощает совместную работу и устранение ошибок.

6. **Развитие DevOps-подхода**: IaaC является ключевым элементом DevOps-подхода к разработке и управлению приложениями. Это способствует интеграции между разработкой и операциями, что улучшает процессы развертывания и обеспечивает более быструю и надежную поставку приложений.

7. **Эффективное использование ресурсов**: IaaC позволяет оптимизировать использование ресурсов, так как вы можете точно настроить конфигурацию инфраструктуры в соответствии с требованиями приложения, без избыточных затрат.

8. **Более безопасная инфраструктура**: IaaC позволяет внедрять лучшие практики безопасности как часть кода инфраструктуры, что делает ее более надежной и защищенной.

Применение IaaC-паттернов существенно улучшает управление и развертывание инфраструктуры в облаке, обеспечивая высокую степень автоматизации, надежности и гибкости, что делает их важным инструментом для современных организаций.

_Какой из принципов IaaC является основополагающим?_

Ответ:

Один из основополагающих принципов IaaC (Infrastructure as Code) - это принцип "Инфраструктура как код". Этот принцип подразумевает, что инфраструктура, используемая для развертывания и управления приложениями, должна быть представлена в виде кода, который можно создавать, изменять, хранить и управлять так же, как и код приложения.

Важными аспектами этого принципа являются:

1. **Автоматизация**: Инфраструктура должна автоматизироваться с использованием сценариев и скриптов, написанных на языке программирования. Это позволяет устранить ручное вмешательство и снизить вероятность ошибок при управлении инфраструктурой.

2. **Управление версиями**: Код инфраструктуры должен храниться в системе управления версиями, такой как Git. Это обеспечивает возможность отслеживания изменений, восстановления предыдущих состояний и совместной работы над инфраструктурным кодом.

3. **Повторяемость**: Инфраструктура должна быть создаваема и воссоздаваема с помощью кода. Это позволяет создавать идентичные среды для разработки, тестирования и продукции, что способствует повторяемости и надежности процессов.

4. **Масштабируемость**: Инфраструктурный код должен быть способен масштабироваться в зависимости от изменяющихся требований. Это означает, что вы можете легко добавлять или удалять ресурсы, чтобы удовлетворить потребности вашего приложения или бизнеса.

Все эти аспекты принципа "Инфраструктура как код" содействуют более эффективному, надежному и гибкому управлению инфраструктурой, что делает его одним из ключевых принципов IaaC.


## Задача 2
_Чем Ansible выгодно отличается от других систем управление конфигурациями?_

Ответ:

Ansible - это популярная система управления конфигурациями и автоматизации, которая предоставляет ряд преимуществ и отличий от других инструментов в этой области:

1. **Простота и читаемость кода**: Ansible использует язык описания конфигурации, который чрезвычайно читаем и понятен. Файлы конфигурации Ansible называются плейбуками и написаны на YAML, что делает их доступными для разработчиков и администраторов, даже если у них нет глубоких знаний в области программирования.

2. **Агентлесс архитектура**: Ansible работает по принципу SSH (или WinRM для Windows) для взаимодействия с удаленными хостами, и не требует установки агентов на целевых системах. Это упрощает развертывание и управление, так как не требуется предварительная установка и настройка на каждом хосте.

3. **Поддержка множества платформ**: Ansible поддерживает множество операционных систем, включая Linux, Windows и другие. Это делает его универсальным инструментом для управления разнообразными окружениями.

4. **Модульность и расширяемость**: Ansible обладает множеством встроенных модулей, которые покрывают широкий спектр задач, от управления конфигурациями до развертывания приложений. Вы также можете создавать собственные модули и расширять функциональность Ansible под свои нужды.

5. **Автоматизация и оркестрация**: Ansible позволяет автоматизировать не только задачи конфигурации, но и процессы оркестрации, такие как развертывание приложений, обновления и масштабирование инфраструктуры.

6. **Сообщество и экосистема**: Ansible имеет активное сообщество пользователей и разработчиков, что обеспечивает доступ к обширной библиотеке плейбуков и ролей. Это позволяет использовать готовые решения для множества задач.

7. **Безопасность**: Ansible предоставляет средства для управления ключами и секретами, что помогает обеспечивать безопасное управление конфигурацией и данными.

8. **Бесплатность и открытый исходный код**: Ansible является проектом с открытым исходным кодом, доступным бесплатно, что делает его доступным для широкого круга организаций и индивидуальных пользователей.

Эти особенности делают Ansible популярным и мощным инструментом для управления конфигурациями и автоматизации задач в инфраструктуре и приложениях.

_Какой, на ваш взгляд, метод работы систем конфигурации более надёжный — push или pull?_

Ответ: 

Выбор между методами push и pull в системах управления конфигурацией зависит от конкретных требований и контекста инфраструктуры. Оба метода имеют свои преимущества и недостатки, и надежность зависит от того, как они реализованы и как хорошо они соответствуют потребностям. Вот краткий обзор каждого метода:

**Push-метод**:
- **Преимущества**:
  1. Простота в настройке и использовании: Push-метод позволяет администраторам отправлять обновления и конфигурации непосредственно на управляемые узлы.
  2. Быстрая реакция на изменения: Изменения могут быть быстро применены на узлах, что полезно в случае срочных обновлений или аварийных ситуаций.
  3. Централизованное управление: Управление изменениями выполняется из одной центральной точки.

- **Недостатки**:
  1. Сложность масштабирования: Push-метод может столкнуться с проблемами масштабирования при управлении большим количеством узлов, особенно если они находятся в разных сетях или зонах.
  2. Ограниченная видимость: Администраторы не всегда имеют полную видимость над состоянием управляемых узлов, пока не отправят на них изменения.

**Pull-метод**:
- **Преимущества**:
  1. Легко масштабируется: Pull-метод может легко масштабироваться для управления большим числом узлов и даже в различных сетях или зонах.
  2. Централизованная видимость: Администраторы имеют более полную видимость и контроль над состоянием всех узлов, так как узлы активно запрашивают конфигурацию.

- **Недостатки**:
  1. Задержка обновлений: Pull-метод может быть несколько медленнее в распространении изменений, так как узлы запрашивают конфигурацию периодически.
  2. Потребление ресурсов: Узлы могут регулярно опрашивать сервер для получения обновлений, что может создать ненужную нагрузку на сеть и сервер.

В целом, надежность метода (push или pull) зависит от специфических требований инфраструктуры, сетевой топологии, размера и распределения узлов, а также сроков обновлений. В некоторых сценариях может быть полезно использовать комбинацию обоих методов (например, push для критических обновлений и pull для регулярной проверки конфигурации). Надежность также зависит от правильной настройки и реализации выбранного метода.

## Задача 3
- Установите на личный компьютер и приложите вывод команд установленных версий каждой из программ, оформленный в Markdown.

Ответ:
```sh
vboxmanage --version
7.0.10r158379
```
```sh
vagrant version
Installed Version: 2.3.7
Latest Version: 2.3.7
```
```sh
terraform -v
Terraform v1.5.7
on darwin_amd64
```
```sh
ansible --version
ansible [core 2.15.3]
  config file = None
  configured module search path = ['/Users/ss/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /usr/local/Cellar/ansible/8.3.0/libexec/lib/python3.11/site-packages/ansible
  ansible collection location = /Users/ss/.ansible/collections:/usr/share/ansible/collections
  executable location = /usr/local/bin/ansible
  python version = 3.11.5 (main, Aug 24 2023, 15:18:16) [Clang 14.0.3 (clang-1403.0.22.14.1)] (/usr/local/Cellar/ansible/8.3.0/libexec/bin/python)
  jinja version = 3.1.2
  libyaml = True
  ```

## Задача 4
Ответ:

![Скриншот](https://github.com/serlukinov/devops-netology/raw/master/image/image.png)

