## Федеративные пользователи {#user-sso}

Если при [настройке федерации](../../organization/concepts/add-federation.md#federation-usage) вы не включили опцию **Автоматически создавать пользователей**, федеративных пользователей нужно добавить в организацию вручную.

Для этого необходимо знать Name ID пользователей, которые вместе с ответом об успешной аутентификации возвращает сервер поставщика удостоверений (IdP). Обычно это электронная почта пользователя. Чтобы узнать, что возвращается в качестве Name ID, обратитесь к администратору, который настраивал аутентификацию в вашей федерации.

{% include [auto-create-users](../../_includes/organization/auto-create-users.md) %}

### Добавьте федеративных пользователей {#add-user-sso}

{% include notitle [user-sso](add-user-sso.md) %}
