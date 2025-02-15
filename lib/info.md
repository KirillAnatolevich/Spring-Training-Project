### Области видимости бинов  
* **Бин-синглтон (Singleton Bean, по умолчанию)** — единственный экземпляр бина в IoC-контейнере Spring. Он создаётся один раз и используется несколькими запросами или ссылками в контексте приложения.

* **Бин-прототип (Prototype Bean)** — новый экземпляр бина, создаваемый каждый раз, когда он запрашивается у IoC-контейнера Spring.

* **Бин запроса (Request Bean)** — связан с жизненным циклом HTTP-запроса в веб-приложениях.

* **Бин сессии (Session Bean)** — связан с жизненным циклом HTTP-сессии в веб-приложениях.

* **Бин приложения (Application Bean)** — связан с жизненным циклом контекста приложения Spring.

Для того, чтобы указать область видимости бина, отличный от singleton, необходимо добавить аннотацию @Scope("область_видимости") методу объявления бина или классу с аннотацией @Component