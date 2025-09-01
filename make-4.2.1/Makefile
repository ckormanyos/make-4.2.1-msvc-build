CC=tcc
CFLAGS=-I. -Iw32/include -Iglob -DHAVE_CONFIG_H=1 -DWINDOWS32=1 -DHAVE_STRNCASECMP -D_cdecl=__cdecl
OBJS=     \
m_ar.o     \
m_arscan.o  \
m_comman.o   \
m_defaul.o \
m_dir.o     \
m_expand.o   \
m_file.o      \
m_functi.o     \
m_getloa.o      \
m_getopt.o \
m_gtopt1.o  \
m_guile.o    \
m_hash.o      \
m_implic.o     \
m_job.o         \
m_load.o         \
m_main.o          \
m_misc.o  \
m_output.o \
m_read.o    \
m_remake.o   \
m_remote.o    \
m_rule.o   \
m_signame.o \
m_strcac.o   \
m_variab.o    \
m_versio.o     \
m_vpath.o \
m_posixf.o \
m_dirent.o  \
m_spmisc.o   \
m_spsubp.o    \
m_spw32e.o \
m_glfnma.o  \
m_glglob.o \
m_w3path.o  \
m_w3w32o.o
DIR_MAKE=./
PS=/
all: make.exe
make.exe: $(OBJS)
	tcc $(OBJS) -o $@ -luser32 -lkernel32 -lgdi32  -lcomdlg32 -ladvapi32 -lshell32 -lole32 -loleaut32 -lodbc32 -lodbccp32
m_ar.o:                $(DIR_MAKE)ar.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)ar.c -o $@
m_arscan.o:            $(DIR_MAKE)arscan.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)arscan.c -o $@
m_comman.o:            $(DIR_MAKE)commands.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)commands.c -o $@
m_defaul.o:            $(DIR_MAKE)default.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)default.c -o $@
m_dir.o    :           $(DIR_MAKE)dir.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)dir.c -o $@
m_expand.o :           $(DIR_MAKE)expand.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)expand.c -o $@
m_file.o   :           $(DIR_MAKE)file.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)file.c -o $@
m_functi.o :           $(DIR_MAKE)function.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)function.c -o $@
m_getloa.o :           $(DIR_MAKE)getloadavg.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)getloadavg.c -o $@
m_getopt.o :           $(DIR_MAKE)getopt.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)getopt.c -o $@
m_gtopt1.o :           $(DIR_MAKE)getopt1.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)getopt1.c -o $@
m_guile.o  :           $(DIR_MAKE)guile.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)guile.c -o $@
m_hash.o   :           $(DIR_MAKE)hash.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)hash.c -o $@
m_implic.o :           $(DIR_MAKE)implicit.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)implicit.c -o $@
m_job.o    :           $(DIR_MAKE)job.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)job.c -o $@
m_load.o   :           $(DIR_MAKE)load.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)load.c -o $@
m_main.o   :           $(DIR_MAKE)main.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)main.c -o $@
m_misc.o   :           $(DIR_MAKE)misc.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)misc.c -o $@
m_output.o :           $(DIR_MAKE)output.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)output.c -o $@
m_read.o   :           $(DIR_MAKE)read.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)read.c -o $@
m_remake.o :           $(DIR_MAKE)remake.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)remake.c -o $@
m_remote.o :           $(DIR_MAKE)remote-stub.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)remote-stub.c -o $@
m_rule.o   :           $(DIR_MAKE)rule.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)rule.c -o $@
m_signame.o:           $(DIR_MAKE)signame.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)signame.c -o $@
m_strcac.o :           $(DIR_MAKE)strcache.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)strcache.c -o $@
m_variab.o :           $(DIR_MAKE)variable.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)variable.c -o $@
m_versio.o :           $(DIR_MAKE)version.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)version.c -o $@
m_vpath.o  :           $(DIR_MAKE)vpath.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)vpath.c -o $@
m_posixf.o:            $(DIR_MAKE)w32$(PS)compat$(PS)posixfcn.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)compat$(PS)posixfcn.c -o $@
m_dirent.o:            $(DIR_MAKE)w32$(PS)compat$(PS)dirent.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)compat$(PS)dirent.c -o $@
m_spmisc.o:            $(DIR_MAKE)w32$(PS)subproc$(PS)misc.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)subproc$(PS)misc.c -o $@
m_spsubp.o:            $(DIR_MAKE)w32$(PS)subproc$(PS)sub_proc.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)subproc$(PS)sub_proc.c -o $@
m_spw32e.o:            $(DIR_MAKE)w32$(PS)subproc$(PS)w32err.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)subproc$(PS)w32err.c -o $@
m_glfnma.o:            $(DIR_MAKE)glob$(PS)fnmatch.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)glob$(PS)fnmatch.c -o $@
m_glglob.o:            $(DIR_MAKE)glob$(PS)glob.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)glob$(PS)glob.c -o $@
m_w3path.o:            $(DIR_MAKE)w32$(PS)pathstuff.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)pathstuff.c -o $@
m_w3w32o.o:            $(DIR_MAKE)w32$(PS)w32os.c
	$(CC) $(CFLAGS) -c $(DIR_MAKE)w32$(PS)w32os.c -o $@
clean:
	del *.o
