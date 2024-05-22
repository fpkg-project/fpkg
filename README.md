# fpkg
fpkg is a (VERY MUCH IN DEVELOPMENT) package management system that enables portable applications to seamlessly share libraries with zero runtime overhead for the applications.
The goal of fpkg is to simplify application distribution such that one can package an application for a platform and have it run perfectly on that platform
regardless of what libraries are available. If something isn't there and a package needs it, it is fetched. If that thing is there, it is made available to the
package. This system of matching dependencies with packages is nothing more than hard links, making it extremely fast and hard to break. If the original
library is deleted, nothing breaks. If you delete fpkg, nothing breaks. If you move an application as a unit from one system to another, which it is actually
quite easy to do, nothing breaks. Fpkg does not use any kind of daemon, kernel patch or any other continuously running system to maintain this. All of the work
happens when you type "fpkg install" (or whatever you do on your frontent of choice).
