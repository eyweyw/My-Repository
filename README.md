# My-Repository
README
License

        Linux kernel release 4.x <http://kernel.org/>

These are the release notes for Linux version 4.  Read them carefully,
as they tell you what this is all about, explain how to install the
kernel, and what to do if something goes wrong. 

WHAT IS LINUX?

  Linux is a clone of the operating system Unix, written from scratch by
  Linus Torvalds with assistance from a loosely-knit team of hackers across
  the Net. It aims towards POSIX and Single UNIX Specification compliance.

  It has all the features you would expect in a modern fully-fledged Unix,
  including true multitasking, virtual memory, shared libraries, demand
  loading, shared copy-on-write executables, proper memory management,
  and multistack networking including IPv4 and IPv6.

  It is distributed under the GNU General Public License - see the
  accompanying COPYING file for more details. 

ON WHAT HARDWARE DOES IT RUN?

  Although originally developed first for 32-bit x86-based PCs (386 or higher),
  today Linux also runs on (at least) the Compaq Alpha AXP, Sun SPARC and
  UltraSPARC, Motorola 68000, PowerPC, PowerPC64, ARM, Hitachi SuperH, Cell,
  IBM S/390, MIPS, HP PA-RISC, Intel IA-64, DEC VAX, AMD x86-64, AXIS CRIS,
  Xtensa, Tilera TILE, AVR32, ARC and Renesas M32R architectures.

  Linux is easily portable to most general-purpose 32- or 64-bit architectures
  as long as they have a paged memory management unit (PMMU) and a port of the
  GNU C compiler (gcc) (part of The GNU Compiler Collection, GCC). Linux has
  also been ported to a number of architectures without a PMMU, although
  functionality is then obviously somewhat limited.
  Linux has also been ported to itself. You can now run the kernel as a
  userspace application - this is called UserMode Linux (UML).

DOCUMENTATION:

 - There is a lot of documentation available both in electronic form on
   the Internet and in books, both Linux-specific and pertaining to
   general UNIX questions.  I'd recommend looking into the documentation
   subdirectories on any Linux FTP site for the LDP (Linux Documentation
   Project) books.  This README is not meant to be documentation on the
   system: there are much better sources available.

 - There are various README files in the Documentation/ subdirectory:
   these typically contain kernel-specific installation notes for some 
   drivers for example. See Documentation/00-INDEX for a list of what
   is contained in each file.  Please read the Changes file, as it
   contains information about the problems, which may result by upgrading
   your kernel.

 - The Documentation/DocBook/ subdirectory contains several guides for
   kernel developers and users.  These guides can be rendered in a
   number of formats:  PostScript (.ps), PDF, HTML, & man-pages, among others.
   After installation, "make psdocs", "make pdfdocs", "make htmldocs",
   or "make mandocs" will render the documentation in the requested format.

INSTALLING the kernel source:

 - If you install the full sources, put the kernel tarball in a
   directory where you have permissions (eg. your home directory) and
   unpack it:

     xz -cd linux-4.X.tar.xz | tar xvf -

   Replace "X" with the version number of the latest kernel.

   Do NOT use the /usr/src/linux area! This area has a (usually
   incomplete) set of kernel headers that are used by the library header
   files.  They should match the library, and not get messed up by
   whatever the kernel-du-jour happens to be.
