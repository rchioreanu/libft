# libft
Creating a homebrew library with most of the libc99 functions and extras

Trace:

= Host-specific information ====================================================
$> hostname; uname -msr
e3r3p12.42.fr
Darwin 15.6.0 x86_64
$> date
Tue Dec 27 12:04:29 CET 2016
$> gcc --version
	Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/usr/include/c++/4.2.1
Apple LLVM version 8.0.0 (clang-800.0.42.1)
	Target: x86_64-apple-darwin15.6.0
	Thread model: posix
	InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
	$> clang --version
Apple LLVM version 8.0.0 (clang-800.0.42.1)
	Target: x86_64-apple-darwin15.6.0
	Thread model: posix
	InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin

	= User files collection ========================================================
	Collecting user files from Vogsphere
	Repository URL: intra/2016/activities/libft/rchiorea

	= Git history ==================================================================
	$> git -C /var/folders/h1/pjl4wxps2pj4x0vcnv41fvzc0000gq/T/tmpq0fLnU/user log --pretty='%H - %an, %ad : %s'
	2d563f236ee30c130c5b68005c6c9744eb17cb6f - Rares CHIOREANU, Fri Dec 23 19:54:42 2016 +0200 : Sfarsit
	284e6837e58312369fd5ff8e73164ba88da58f04 - Rares CHIOREANU, Thu Dec 22 20:40:00 2016 +0200 : first day

	= Collected files ==========================================
	$> ls -lAR /var/folders/h1/pjl4wxps2pj4x0vcnv41fvzc0000gq/T/tmpq0fLnU/user
	total 520
	-rw-r--r--  1 deepthought  deepthought      0 Dec 27 12:04 .nfs.20051080.0118
	-rw-r--r--  1 deepthought  deepthought  12288 Dec 27 12:04 .nfs.20051081.0122
	-rw-r--r--  1 deepthought  deepthought   1870 Dec 27 12:04 Makefile
	-rw-r--r--  1 deepthought  deepthought   3811 Dec 27 12:04 __GIT_HISTORY
	-rw-r--r--  1 deepthought  deepthought      9 Dec 27 12:04 auteur
	-rw-r--r--  1 deepthought  deepthought   1237 Dec 27 12:04 ft_atoi.c
	-rw-r--r--  1 deepthought  deepthought   1064 Dec 27 12:04 ft_bzero.c
	-rw-r--r--  1 deepthought  deepthought   1056 Dec 27 12:04 ft_isalnum.c
	-rw-r--r--  1 deepthought  deepthought   1020 Dec 27 12:04 ft_isalpha.c
	-rw-r--r--  1 deepthought  deepthought    997 Dec 27 12:04 ft_isascii.c
	-rw-r--r--  1 deepthought  deepthought    999 Dec 27 12:04 ft_isdigit.c
	-rw-r--r--  1 deepthought  deepthought    997 Dec 27 12:04 ft_isprint.c
	-rw-r--r--  1 deepthought  deepthought   1863 Dec 27 12:04 ft_itoa.c
	-rw-r--r--  1 deepthought  deepthought   1016 Dec 27 12:04 ft_lstadd.c
	-rw-r--r--  1 deepthought  deepthought   1123 Dec 27 12:04 ft_lstdel.c
	-rw-r--r--  1 deepthought  deepthought   1054 Dec 27 12:04 ft_lstdelone.c
	-rw-r--r--  1 deepthought  deepthought   1026 Dec 27 12:04 ft_lstiter.c
	-rw-r--r--  1 deepthought  deepthought   1292 Dec 27 12:04 ft_lstmap.c
	-rw-r--r--  1 deepthought  deepthought   1359 Dec 27 12:04 ft_lstnew.c
	-rw-r--r--  1 deepthought  deepthought   1080 Dec 27 12:04 ft_memalloc.c
	-rw-r--r--  1 deepthought  deepthought   1263 Dec 27 12:04 ft_memccpy.c
	-rw-r--r--  1 deepthought  deepthought   1126 Dec 27 12:04 ft_memchr.c
	-rw-r--r--  1 deepthought  deepthought   1229 Dec 27 12:04 ft_memcmp.c
	-rw-r--r--  1 deepthought  deepthought   1163 Dec 27 12:04 ft_memcpy.c
	-rw-r--r--  1 deepthought  deepthought    964 Dec 27 12:04 ft_memdel.c
	-rw-r--r--  1 deepthought  deepthought   1233 Dec 27 12:04 ft_memmove.c
	-rw-r--r--  1 deepthought  deepthought   1098 Dec 27 12:04 ft_memset.c
	-rw-r--r--  1 deepthought  deepthought    958 Dec 27 12:04 ft_putchar.c
	-rw-r--r--  1 deepthought  deepthought    970 Dec 27 12:04 ft_putchar_fd.c
	-rw-r--r--  1 deepthought  deepthought   1030 Dec 27 12:04 ft_putendl.c
	-rw-r--r--  1 deepthought  deepthought   1058 Dec 27 12:04 ft_putendl_fd.c
	-rw-r--r--  1 deepthought  deepthought    962 Dec 27 12:04 ft_putnbr.c
	-rw-r--r--  1 deepthought  deepthought    980 Dec 27 12:04 ft_putnbr_fd.c
	-rw-r--r--  1 deepthought  deepthought   1013 Dec 27 12:04 ft_putstr.c
	-rw-r--r--  1 deepthought  deepthought   1031 Dec 27 12:04 ft_putstr_fd.c
	-rw-r--r--  1 deepthought  deepthought   1113 Dec 27 12:04 ft_strcat.c
	-rw-r--r--  1 deepthought  deepthought   1110 Dec 27 12:04 ft_strchr.c
	-rw-r--r--  1 deepthought  deepthought   1002 Dec 27 12:04 ft_strclr.c
	-rw-r--r--  1 deepthought  deepthought   1154 Dec 27 12:04 ft_strcmp.c
	-rw-r--r--  1 deepthought  deepthought   1085 Dec 27 12:04 ft_strcpy.c
	-rw-r--r--  1 deepthought  deepthought    964 Dec 27 12:04 ft_strdel.c
	-rw-r--r--  1 deepthought  deepthought   1133 Dec 27 12:04 ft_strdup.c
	-rw-r--r--  1 deepthought  deepthought   1136 Dec 27 12:04 ft_strequ.c
	-rw-r--r--  1 deepthought  deepthought   1008 Dec 27 12:04 ft_striter.c
	-rw-r--r--  1 deepthought  deepthought   1065 Dec 27 12:04 ft_striteri.c
	-rw-r--r--  1 deepthought  deepthought   1291 Dec 27 12:04 ft_strjoin.c
	-rw-r--r--  1 deepthought  deepthought   1289 Dec 27 12:04 ft_strlcat.c
	-rw-r--r--  1 deepthought  deepthought   1010 Dec 27 12:04 ft_strlen.c
	-rw-r--r--  1 deepthought  deepthought   1153 Dec 27 12:04 ft_strmap.c
	-rw-r--r--  1 deepthought  deepthought   1179 Dec 27 12:04 ft_strmapi.c
	-rw-r--r--  1 deepthought  deepthought   1133 Dec 27 12:04 ft_strncat.c
	-rw-r--r--  1 deepthought  deepthought   1222 Dec 27 12:04 ft_strncmp.c
	-rw-r--r--  1 deepthought  deepthought   1112 Dec 27 12:04 ft_strncpy.c
	-rw-r--r--  1 deepthought  deepthought   1109 Dec 27 12:04 ft_strnequ.c
	-rw-r--r--  1 deepthought  deepthought   1091 Dec 27 12:04 ft_strnew.c
	-rw-r--r--  1 deepthought  deepthought   1238 Dec 27 12:04 ft_strnstr.c
	-rw-r--r--  1 deepthought  deepthought   1098 Dec 27 12:04 ft_strrchr.c
	-rw-r--r--  1 deepthought  deepthought   1763 Dec 27 12:04 ft_strsplit.c
	-rw-r--r--  1 deepthought  deepthought   1285 Dec 27 12:04 ft_strstr.c
	-rw-r--r--  1 deepthought  deepthought   1165 Dec 27 12:04 ft_strsub.c
	-rw-r--r--  1 deepthought  deepthought   1293 Dec 27 12:04 ft_strtrim.c
	-rw-r--r--  1 deepthought  deepthought   1016 Dec 27 12:04 ft_tolower.c
	-rw-r--r--  1 deepthought  deepthought   1023 Dec 27 12:04 ft_toupper.c
	-rw-r--r--  1 deepthought  deepthought   3705 Dec 27 12:04 libft.h

	= libft_basics_1 ===============================================================
	/bin/rm -f *.o
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	/bin/rm -f *.o
	/bin/rm -f libft.a libft.so
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	/bin/rm -f *.o
	/bin/rm -f libft.a libft.so
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	-rw-r--r--  1 deepthought  deepthought  52496 Dec 27 12:04 libft.a

	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_atoi.o test_ft_atoi.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_bzero.o test_ft_bzero.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_isalnum.o test_ft_isalnum.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_isalpha.o test_ft_isalpha.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_isascii.o test_ft_isascii.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_isdigit.o test_ft_isdigit.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_isprint.o test_ft_isprint.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memccpy.o test_ft_memccpy.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memchr.o test_ft_memchr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memcmp.o test_ft_memcmp.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memcpy.o test_ft_memcpy.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memmove.o test_ft_memmove.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memset.o test_ft_memset.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strcat.o test_ft_strcat.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strchr.o test_ft_strchr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strcmp.o test_ft_strcmp.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strcpy.o test_ft_strcpy.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strdup.o test_ft_strdup.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strlcat.o test_ft_strlcat.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strlen.o test_ft_strlen.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strncat.o test_ft_strncat.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strncmp.o test_ft_strncmp.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strncpy.o test_ft_strncpy.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strnstr.o test_ft_strnstr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strrchr.o test_ft_strrchr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strstr.o test_ft_strstr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_tolower.o test_ft_tolower.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_toupper.o test_ft_toupper.c
	gcc -Wall -Wextra -Werror -g3   -c -o main.o main.c
	gcc -Wall -Wextra -Werror -g3 -o test_lib -L. -lft test_ft_atoi.o test_ft_bzero.o test_ft_isalnum.o test_ft_isalpha.o test_ft_isascii.o test_ft_isdigit.o test_ft_isprint.o test_ft_memccpy.o test_ft_memchr.o test_ft_memcmp.o test_ft_memcpy.o test_ft_memmove.o test_ft_memset.o test_ft_strcat.o test_ft_strchr.o test_ft_strcmp.o test_ft_strcpy.o test_ft_strdup.o test_ft_strlcat.o test_ft_strlen.o test_ft_strncat.o test_ft_strncmp.o test_ft_strncpy.o test_ft_strnstr.o test_ft_strrchr.o test_ft_strstr.o test_ft_tolower.o test_ft_toupper.o main.o


	ft_atoi: [ok]
	ft_bzero: [ok]
	ft_isalnum: [ok]
	ft_isalpha: [ok]
	ft_isascii: [ok]
	ft_isdigit: [ok]
	ft_isprint: [ok]
	ft_memccpy: [ok]
	ft_memchr: [ok]
	ft_memcmp: [ok]
	ft_memcpy: [ok]
	ft_memmove: [ok]
	ft_memset: [ok]
	ft_strcat: [ok]
	ft_strchr: [ok]
	ft_strcmp: [ok]
	ft_strcpy: [ok]
	ft_strdup: [ok]
	ft_strlcat: [ok]
	ft_strlen: [ok]
	ft_strncat: [ok]
	ft_strncmp: [ok]
	ft_strncpy: [ok]
	ft_strnstr: [ok]
	ft_strrchr: [ok]
	ft_strstr: [ok]
	ft_tolower: [ok]
	ft_toupper: [ok]

	28/28 correct functions
	Grade: 60

	= libft_basics_2 ===============================================================
	total 480
	-rw-r--r--  1 deepthought  deepthought  1870 Dec 27 12:04 Makefile
	-rw-r--r--  1 deepthought  deepthought  1237 Dec 27 12:04 ft_atoi.c
	-rw-r--r--  1 deepthought  deepthought  1064 Dec 27 12:04 ft_bzero.c
	-rw-r--r--  1 deepthought  deepthought  1056 Dec 27 12:04 ft_isalnum.c
	-rw-r--r--  1 deepthought  deepthought  1020 Dec 27 12:04 ft_isalpha.c
	-rw-r--r--  1 deepthought  deepthought   997 Dec 27 12:04 ft_isascii.c
	-rw-r--r--  1 deepthought  deepthought   999 Dec 27 12:04 ft_isdigit.c
	-rw-r--r--  1 deepthought  deepthought   997 Dec 27 12:04 ft_isprint.c
	-rw-r--r--  1 deepthought  deepthought  1863 Dec 27 12:04 ft_itoa.c
	-rw-r--r--  1 deepthought  deepthought  1016 Dec 27 12:04 ft_lstadd.c
	-rw-r--r--  1 deepthought  deepthought  1123 Dec 27 12:04 ft_lstdel.c
	-rw-r--r--  1 deepthought  deepthought  1054 Dec 27 12:04 ft_lstdelone.c
	-rw-r--r--  1 deepthought  deepthought  1026 Dec 27 12:04 ft_lstiter.c
	-rw-r--r--  1 deepthought  deepthought  1292 Dec 27 12:04 ft_lstmap.c
	-rw-r--r--  1 deepthought  deepthought  1359 Dec 27 12:04 ft_lstnew.c
	-rw-r--r--  1 deepthought  deepthought  1080 Dec 27 12:04 ft_memalloc.c
	-rw-r--r--  1 deepthought  deepthought  1263 Dec 27 12:04 ft_memccpy.c
	-rw-r--r--  1 deepthought  deepthought  1126 Dec 27 12:04 ft_memchr.c
	-rw-r--r--  1 deepthought  deepthought  1229 Dec 27 12:04 ft_memcmp.c
	-rw-r--r--  1 deepthought  deepthought  1163 Dec 27 12:04 ft_memcpy.c
	-rw-r--r--  1 deepthought  deepthought   964 Dec 27 12:04 ft_memdel.c
	-rw-r--r--  1 deepthought  deepthought  1233 Dec 27 12:04 ft_memmove.c
	-rw-r--r--  1 deepthought  deepthought  1098 Dec 27 12:04 ft_memset.c
	-rw-r--r--  1 deepthought  deepthought   958 Dec 27 12:04 ft_putchar.c
	-rw-r--r--  1 deepthought  deepthought   970 Dec 27 12:04 ft_putchar_fd.c
	-rw-r--r--  1 deepthought  deepthought  1030 Dec 27 12:04 ft_putendl.c
	-rw-r--r--  1 deepthought  deepthought  1058 Dec 27 12:04 ft_putendl_fd.c
	-rw-r--r--  1 deepthought  deepthought   962 Dec 27 12:04 ft_putnbr.c
	-rw-r--r--  1 deepthought  deepthought   980 Dec 27 12:04 ft_putnbr_fd.c
	-rw-r--r--  1 deepthought  deepthought  1013 Dec 27 12:04 ft_putstr.c
	-rw-r--r--  1 deepthought  deepthought  1031 Dec 27 12:04 ft_putstr_fd.c
	-rw-r--r--  1 deepthought  deepthought  1113 Dec 27 12:04 ft_strcat.c
	-rw-r--r--  1 deepthought  deepthought  1110 Dec 27 12:04 ft_strchr.c
	-rw-r--r--  1 deepthought  deepthought  1002 Dec 27 12:04 ft_strclr.c
	-rw-r--r--  1 deepthought  deepthought  1154 Dec 27 12:04 ft_strcmp.c
	-rw-r--r--  1 deepthought  deepthought  1085 Dec 27 12:04 ft_strcpy.c
	-rw-r--r--  1 deepthought  deepthought   964 Dec 27 12:04 ft_strdel.c
	-rw-r--r--  1 deepthought  deepthought  1133 Dec 27 12:04 ft_strdup.c
	-rw-r--r--  1 deepthought  deepthought  1136 Dec 27 12:04 ft_strequ.c
	-rw-r--r--  1 deepthought  deepthought  1008 Dec 27 12:04 ft_striter.c
	-rw-r--r--  1 deepthought  deepthought  1065 Dec 27 12:04 ft_striteri.c
	-rw-r--r--  1 deepthought  deepthought  1291 Dec 27 12:04 ft_strjoin.c
	-rw-r--r--  1 deepthought  deepthought  1289 Dec 27 12:04 ft_strlcat.c
	-rw-r--r--  1 deepthought  deepthought  1010 Dec 27 12:04 ft_strlen.c
	-rw-r--r--  1 deepthought  deepthought  1153 Dec 27 12:04 ft_strmap.c
	-rw-r--r--  1 deepthought  deepthought  1179 Dec 27 12:04 ft_strmapi.c
	-rw-r--r--  1 deepthought  deepthought  1133 Dec 27 12:04 ft_strncat.c
	-rw-r--r--  1 deepthought  deepthought  1222 Dec 27 12:04 ft_strncmp.c
	-rw-r--r--  1 deepthought  deepthought  1112 Dec 27 12:04 ft_strncpy.c
	-rw-r--r--  1 deepthought  deepthought  1109 Dec 27 12:04 ft_strnequ.c
	-rw-r--r--  1 deepthought  deepthought  1091 Dec 27 12:04 ft_strnew.c
	-rw-r--r--  1 deepthought  deepthought  1238 Dec 27 12:04 ft_strnstr.c
	-rw-r--r--  1 deepthought  deepthought  1098 Dec 27 12:04 ft_strrchr.c
	-rw-r--r--  1 deepthought  deepthought  1763 Dec 27 12:04 ft_strsplit.c
	-rw-r--r--  1 deepthought  deepthought  1285 Dec 27 12:04 ft_strstr.c
	-rw-r--r--  1 deepthought  deepthought  1165 Dec 27 12:04 ft_strsub.c
	-rw-r--r--  1 deepthought  deepthought  1293 Dec 27 12:04 ft_strtrim.c
	-rw-r--r--  1 deepthought  deepthought  1016 Dec 27 12:04 ft_tolower.c
	-rw-r--r--  1 deepthought  deepthought  1023 Dec 27 12:04 ft_toupper.c
	-rw-r--r--  1 deepthought  deepthought  3705 Dec 27 12:04 libft.h
	/bin/rm -f *.o
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	/bin/rm -f *.o
	/bin/rm -f libft.a libft.so
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	/bin/rm -f *.o
	/bin/rm -f libft.a libft.so
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	-rw-r--r--  1 deepthought  deepthought  52496 Dec 27 12:04 libft.a

	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strnew.o test_ft_strnew.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strdel.o test_ft_strdel.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strclr.o test_ft_strclr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_striter.o test_ft_striter.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_striteri.o test_ft_striteri.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strmap.o test_ft_strmap.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strmapi.o test_ft_strmapi.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strequ.o test_ft_strequ.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strnequ.o test_ft_strnequ.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strsub.o test_ft_strsub.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strjoin.o test_ft_strjoin.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strtrim.o test_ft_strtrim.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_strsplit.o test_ft_strsplit.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_itoa.o test_ft_itoa.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putstr.o test_ft_putstr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putchar.o test_ft_putchar.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putendl.o test_ft_putendl.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putnbr.o test_ft_putnbr.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putchar_fd.o test_ft_putchar_fd.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putendl_fd.o test_ft_putendl_fd.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putnbr_fd.o test_ft_putnbr_fd.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_putstr_fd.o test_ft_putstr_fd.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memalloc.o test_ft_memalloc.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_memdel.o test_ft_memdel.c
	gcc -Wall -Wextra -Werror -g3   -c -o main.o main.c
	gcc -Wall -Wextra -Werror -g3 -o test_lib -L. -lft test_ft_strnew.o test_ft_strdel.o test_ft_strclr.o test_ft_striter.o test_ft_striteri.o test_ft_strmap.o test_ft_strmapi.o test_ft_strequ.o test_ft_strnequ.o test_ft_strsub.o test_ft_strjoin.o test_ft_strtrim.o test_ft_strsplit.o test_ft_itoa.o test_ft_putstr.o test_ft_putchar.o test_ft_putendl.o test_ft_putnbr.o test_ft_putchar_fd.o test_ft_putendl_fd.o test_ft_putnbr_fd.o test_ft_putstr_fd.o test_ft_memalloc.o test_ft_memdel.o main.o

	ft_memalloc: [ok]
	ft_memdel: [ok]
	ft_strnew: [ok]
	ft_strdel: [ok]
	ft_strclr: [ok]
	ft_striter: [ok]
	ft_striteri: [ok]
	ft_strmap: [ok]
	ft_strmapi: [ok]
	ft_strequ: [ok]
	ft_strnequ: [ok]
	ft_strsub: [ok]
	ft_strjoin: [ok]
	ft_strtrim: [ok]
	ft_strsplit: [ok]
	ft_itoa: [ok]
	ft_putchar: [ok]
	ft_putstr: [ok]
	ft_putendl: [ok]
	ft_putnbr: [ok]
	ft_putcharfd: [ok]
	ft_putstrfd: [ok]
	ft_putendlfd: [ok]
	ft_putnbrfd: [ok]

	24/24 correct functions
	Grade: 40

	= libft_bonus ==================================================================
	total 480
	-rw-r--r--  1 deepthought  deepthought  1870 Dec 27 12:04 Makefile
	-rw-r--r--  1 deepthought  deepthought  1237 Dec 27 12:04 ft_atoi.c
	-rw-r--r--  1 deepthought  deepthought  1064 Dec 27 12:04 ft_bzero.c
	-rw-r--r--  1 deepthought  deepthought  1056 Dec 27 12:04 ft_isalnum.c
	-rw-r--r--  1 deepthought  deepthought  1020 Dec 27 12:04 ft_isalpha.c
	-rw-r--r--  1 deepthought  deepthought   997 Dec 27 12:04 ft_isascii.c
	-rw-r--r--  1 deepthought  deepthought   999 Dec 27 12:04 ft_isdigit.c
	-rw-r--r--  1 deepthought  deepthought   997 Dec 27 12:04 ft_isprint.c
	-rw-r--r--  1 deepthought  deepthought  1863 Dec 27 12:04 ft_itoa.c
	-rw-r--r--  1 deepthought  deepthought  1016 Dec 27 12:04 ft_lstadd.c
	-rw-r--r--  1 deepthought  deepthought  1123 Dec 27 12:04 ft_lstdel.c
	-rw-r--r--  1 deepthought  deepthought  1054 Dec 27 12:04 ft_lstdelone.c
	-rw-r--r--  1 deepthought  deepthought  1026 Dec 27 12:04 ft_lstiter.c
	-rw-r--r--  1 deepthought  deepthought  1292 Dec 27 12:04 ft_lstmap.c
	-rw-r--r--  1 deepthought  deepthought  1359 Dec 27 12:04 ft_lstnew.c
	-rw-r--r--  1 deepthought  deepthought  1080 Dec 27 12:04 ft_memalloc.c
	-rw-r--r--  1 deepthought  deepthought  1263 Dec 27 12:04 ft_memccpy.c
	-rw-r--r--  1 deepthought  deepthought  1126 Dec 27 12:04 ft_memchr.c
	-rw-r--r--  1 deepthought  deepthought  1229 Dec 27 12:04 ft_memcmp.c
	-rw-r--r--  1 deepthought  deepthought  1163 Dec 27 12:04 ft_memcpy.c
	-rw-r--r--  1 deepthought  deepthought   964 Dec 27 12:04 ft_memdel.c
	-rw-r--r--  1 deepthought  deepthought  1233 Dec 27 12:04 ft_memmove.c
	-rw-r--r--  1 deepthought  deepthought  1098 Dec 27 12:04 ft_memset.c
	-rw-r--r--  1 deepthought  deepthought   958 Dec 27 12:04 ft_putchar.c
	-rw-r--r--  1 deepthought  deepthought   970 Dec 27 12:04 ft_putchar_fd.c
	-rw-r--r--  1 deepthought  deepthought  1030 Dec 27 12:04 ft_putendl.c
	-rw-r--r--  1 deepthought  deepthought  1058 Dec 27 12:04 ft_putendl_fd.c
	-rw-r--r--  1 deepthought  deepthought   962 Dec 27 12:04 ft_putnbr.c
	-rw-r--r--  1 deepthought  deepthought   980 Dec 27 12:04 ft_putnbr_fd.c
	-rw-r--r--  1 deepthought  deepthought  1013 Dec 27 12:04 ft_putstr.c
	-rw-r--r--  1 deepthought  deepthought  1031 Dec 27 12:04 ft_putstr_fd.c
	-rw-r--r--  1 deepthought  deepthought  1113 Dec 27 12:04 ft_strcat.c
	-rw-r--r--  1 deepthought  deepthought  1110 Dec 27 12:04 ft_strchr.c
	-rw-r--r--  1 deepthought  deepthought  1002 Dec 27 12:04 ft_strclr.c
	-rw-r--r--  1 deepthought  deepthought  1154 Dec 27 12:04 ft_strcmp.c
	-rw-r--r--  1 deepthought  deepthought  1085 Dec 27 12:04 ft_strcpy.c
	-rw-r--r--  1 deepthought  deepthought   964 Dec 27 12:04 ft_strdel.c
	-rw-r--r--  1 deepthought  deepthought  1133 Dec 27 12:04 ft_strdup.c
	-rw-r--r--  1 deepthought  deepthought  1136 Dec 27 12:04 ft_strequ.c
	-rw-r--r--  1 deepthought  deepthought  1008 Dec 27 12:04 ft_striter.c
	-rw-r--r--  1 deepthought  deepthought  1065 Dec 27 12:04 ft_striteri.c
	-rw-r--r--  1 deepthought  deepthought  1291 Dec 27 12:04 ft_strjoin.c
	-rw-r--r--  1 deepthought  deepthought  1289 Dec 27 12:04 ft_strlcat.c
	-rw-r--r--  1 deepthought  deepthought  1010 Dec 27 12:04 ft_strlen.c
	-rw-r--r--  1 deepthought  deepthought  1153 Dec 27 12:04 ft_strmap.c
	-rw-r--r--  1 deepthought  deepthought  1179 Dec 27 12:04 ft_strmapi.c
	-rw-r--r--  1 deepthought  deepthought  1133 Dec 27 12:04 ft_strncat.c
	-rw-r--r--  1 deepthought  deepthought  1222 Dec 27 12:04 ft_strncmp.c
	-rw-r--r--  1 deepthought  deepthought  1112 Dec 27 12:04 ft_strncpy.c
	-rw-r--r--  1 deepthought  deepthought  1109 Dec 27 12:04 ft_strnequ.c
	-rw-r--r--  1 deepthought  deepthought  1091 Dec 27 12:04 ft_strnew.c
	-rw-r--r--  1 deepthought  deepthought  1238 Dec 27 12:04 ft_strnstr.c
	-rw-r--r--  1 deepthought  deepthought  1098 Dec 27 12:04 ft_strrchr.c
	-rw-r--r--  1 deepthought  deepthought  1763 Dec 27 12:04 ft_strsplit.c
	-rw-r--r--  1 deepthought  deepthought  1285 Dec 27 12:04 ft_strstr.c
	-rw-r--r--  1 deepthought  deepthought  1165 Dec 27 12:04 ft_strsub.c
	-rw-r--r--  1 deepthought  deepthought  1293 Dec 27 12:04 ft_strtrim.c
	-rw-r--r--  1 deepthought  deepthought  1016 Dec 27 12:04 ft_tolower.c
	-rw-r--r--  1 deepthought  deepthought  1023 Dec 27 12:04 ft_toupper.c
	-rw-r--r--  1 deepthought  deepthought  3705 Dec 27 12:04 libft.h
	/bin/rm -f *.o
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	/bin/rm -f *.o
	/bin/rm -f libft.a libft.so
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	/bin/rm -f *.o
	/bin/rm -f libft.a libft.so
	gcc -c -Wall -Wextra -Werror ft_isalnum.c ft_isprint.c ft_memchr.c ft_memmove.c ft_putendl.c ft_putstr.c ft_strclr.c ft_strdup.c ft_strjoin.c ft_strmapi.c ft_strnequ.c ft_strstr.c ft_toupper.c ft_isalpha.c ft_itoa.c ft_memcmp.c ft_memset.c ft_putendl_fd.c ft_putstr_fd.c ft_strcmp.c ft_strequ.c ft_strlcat.c ft_strncat.c        ft_strnew.c ft_strsub.c ft_atoi.c ft_isascii.c  ft_memalloc.c ft_memcpy.c ft_putchar.c ft_putnbr.c ft_strcat.c ft_strcpy.c ft_striter.c ft_strlen.c ft_strncmp.c ft_strnstr.c ft_strtrim.c ft_bzero.c ft_isdigit.c ft_memccpy.c ft_memdel.c ft_putchar_fd.c ft_putnbr_fd.c ft_strchr.c ft_strdel.c ft_striteri.c ft_strmap.c ft_strncpy.c ft_strrchr.c ft_tolower.c ft_lstnew.c ft_lstadd.c ft_lstdel.c ft_lstdelone.c ft_lstmap.c ft_lstiter.c ft_strsplit.c
	ar rc libft.a ft_isalnum.o ft_isprint.o ft_memchr.o ft_memmove.o ft_putendl.o ft_putstr.o ft_strclr.o ft_strdup.o ft_strjoin.o ft_strmapi.o ft_strnequ.o ft_strstr.o ft_toupper.o ft_isalpha.o ft_itoa.o ft_memcmp.o ft_memset.o ft_putendl_fd.o ft_putstr_fd.o ft_strcmp.o ft_strequ.o ft_strlcat.o ft_strncat.o ft_strnew.o ft_strsub.o ft_atoi.o ft_isascii.o ft_memalloc.o ft_memcpy.o ft_putchar.o ft_putnbr.o ft_strcat.o ft_strcpy.o ft_striter.o ft_strlen.o ft_strncmp.o ft_strnstr.o ft_strtrim.o ft_bzero.o ft_isdigit.o ft_memccpy.o ft_memdel.o ft_putchar_fd.o ft_putnbr_fd.o ft_strchr.o ft_strdel.o ft_striteri.o ft_strmap.o ft_strncpy.o ft_strrchr.o ft_tolower.o ft_lstnew.o ft_lstadd.o ft_lstdel.o ft_lstdelone.o ft_lstmap.o ft_lstiter.o ft_strsplit.o
	ranlib libft.a
	-rw-r--r--  1 deepthought  deepthought  52496 Dec 27 12:04 libft.a

	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_lstadd.o test_ft_lstadd.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_lstdel.o test_ft_lstdel.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_lstdelone.o test_ft_lstdelone.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_lstiter.o test_ft_lstiter.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_lstmap.o test_ft_lstmap.c
	gcc -Wall -Wextra -Werror -g3   -c -o test_ft_lstnew.o test_ft_lstnew.c
	gcc -Wall -Wextra -Werror -g3   -c -o main.o main.c
	gcc -Wall -Wextra -Werror -g3 -o test_lib -L. -lft test_ft_lstadd.o test_ft_lstdel.o test_ft_lstdelone.o test_ft_lstiter.o test_ft_lstmap.o test_ft_lstnew.o main.o

	ft_lstadd: [ok]
	ft_lstdel: [ok]
	ft_lstdelone: [ok]
	ft_lstdeliter: [ok]
	ft_lstmap: [ok]
	ft_lstnew: [ok]

	6/6 correct functions
	Grade: 25

	= Final grade: 125 =============================================================
