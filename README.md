{% global reason = arguments.after(2) %}
📜 | *REPORT*                                                
Был отправлен [репорт ]({{ message.jumpUrl }}) на пользователя / Сообщение {{ arguments.get(1) }}
пользователем {{member.mention}} .

Тект жалобы: {{ reason }}

Прикрепленные файлы: {{message.attachments}}
{% do sourceChannel.sendMessage(format('%s, *Ваша жалоба была отправлена, ожидайте ответ от модерации / Администрации в лс!*  ', member)) %}
