
LOCALS := fr es_ES de_DE it pt_BR zh_CN zh_TW
all:
	@for local in $(LOCALS); do \
        	mkdir -p locale/$$local/LC_MESSAGES/; \
	done

	msgfmt gdm3setup-fr.po -o locale/fr/LC_MESSAGES/gdm3setup.mo
	msgfmt gdm3setup-es_ES.po -o locale/es_ES/LC_MESSAGES/gdm3setup.mo
	msgfmt gdm3setup-de_DE.po -o locale/de_DE/LC_MESSAGES/gdm3setup.mo
	msgfmt gdm3setup-it.po -o locale/it/LC_MESSAGES/gdm3setup.mo
	msgfmt gdm3setup-pt_BR.po -o locale/pt_BR/LC_MESSAGES/gdm3setup.mo
	msgfmt gdm3setup-zh_CN.po -o locale/zh_CN/LC_MESSAGES/gdm3setup.mo
	msgfmt gdm3setup-zh_TW.po -o locale/zh_TW/LC_MESSAGES/gdm3setup.mo

clean:
	rm -r locale

install:
	cp -r locale $(DESTDIR)/usr/share/

uninstall:
	rm $(DESTDIR)/usr/share/locale/{de_DE,es_ES,fr,it,pt_BR,zh_CN,zh_TW}/LC_MESSAGES/gdm3setup.mo



