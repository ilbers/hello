DB2MAN = docbook-to-man
RM = rm

bin_PROGRAMS = hello-isar
hello_isar_SOURCES = hello.c
hello_isar_LDADD = -lhello
man1_MANS = hello-isar.1

hello-isar.1: hello.sgml
	$(DB2MAN) $< >$@

clean-local:
	$(RM) -f $(man1_MANS)
