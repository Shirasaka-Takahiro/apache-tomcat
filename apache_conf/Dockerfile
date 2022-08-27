FROM httpd:alpine
RUN touch /usr/local/apache2/conf/extra/httpd-proxy.conf
RUN echo 'ProxyPass / ajp://tomcat-container:8009/' > /usr/local/apache2/conf/extra/httpd-proxy.conf
RUN mkdir /usr/local/apache2/conf/extra/vhosts
RUN touch /usr/local/apache2/conf/extra/vhosts/hoge.example.com.conf
RUN mkdir -p /usr/local/apache2/sites-enabled/hoge.example.com
RUN touch /usr/local/apache2/sites-enabled/hoge.example.com/index.html
RUN echo 'hoge.example.com' >> /usr/local/apache2/sites-enabled/hoge.example.com/index.html
