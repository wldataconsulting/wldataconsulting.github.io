{% for work in site.work %}
                    {% if work.featured %}
                        {% assign mod = forloop.index | modulo:2 %}
                        {% if mod == 0 %}
                            <a href="{{work.url}}"><div class="col-xs-12 col-md-6 col-md-offset-5 featured-work">
                                <div class="featured-work-title">{{work.title|replace: " ","</br>"}}</div>
                                <div class="featured-work-image" style="background-image: url(/images/{{work.image}});"></div>
                            </div></a>
                        {% else %}
                            <a href="{{work.url}}"><div class="col-xs-12 col-md-6 featured-work">
                                <div class="featured-work-title">{{work.title|replace: " ","</br>"}}</div>
                                <div class="featured-work-image" style="background-image: url(/images/{{work.image}});"></div>
                            </div></a>
                        {% endif %}
                    {% endif %}
{% endfor %}