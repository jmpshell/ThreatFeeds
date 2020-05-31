

	{% for post in site.posts %}
		<entry>
			<title>{{ post.title }}</title>
			<link href="http://hankquinlan.github.io{{ post.url }}"/>
			<updated>{{ post.date | date_to_xmlschema }}</updated>
			<id>http://hankquinlan.github.io{{ post.id }}</id>
			<content type="html">{{ post.content | xml_escape }}</content>
		</entry>
	{% endfor %}

