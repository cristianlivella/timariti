# Timariti
## Online magazines viewer
### 🚧 Just an idea, work in progress

As a webmaster of the [Oratorio Paladina website](https://oratoriopaladina.it/), I'm also in charge to publish the parish magazine on it.

The magazine is primarly intended for print and physical distribution, so the publication on the website is just a secondary aim.

For this reason, the magazine is published online as a PDF file (the same used for printing), that the user can download, or view online using the [Issuu](https://issuu.com/) flipbook viewer.

This looks fine, but in the years I realized that is not a great solution, as continuous zoom in, zoom out and pan are required to read it.

So for a publication, I tried an [hybrid publication method](https://oratoriopaladina.it/2018/08/09/camminiamo-insieme-9/): I still published the original PDF file and the Issuu viewer, but I also published every article as a Wordpress post, and linked them in the publication page.

As I had expected, this drastically increased the fruability of the publication, and in fact it received a lot more views than the others.

With the analytics tools of Wordpress, I also found that months after publication, there are many more visits to individual articles, compared to the full publication. This is probably due to the fact that in this way you can search for articles directly on the site, without having to scroll the PDF, and in this way the articles are also indexed by Google, so they are also read by people who would never have found them otherwise.

This solution looked pretty good, but not good enaugh for me. There are some problems:
- firstly, in recent years Issuu no longer allows you to view the publication directly with their embedded viewer, with the free plan, but requires you to enter their site. This is a degradation to the user experience;
- using Wordpress posts, the original PDF and the posts are completely decoupled, and it's not always easy to let the user know that he is reading a post that is part of a pubblication, and so he can read also the other articles, or view/print the article in the original printed format.

So my idea is to make a platform from scratch that allows for publishing magazines (or similiar contents) with their original PDF files, and the hypertext version for each article, allowing the user to choose which format wants to read, with a better integration between them.

Also, the idea is to make it a platform with (almost) no backend, in fact all the contents are going to be stored in GitHub repositories (especially for hypertexts and configs, while big assets like PDF files and images are going to be uploaded on a web server, or on the [IPFS](https://ipfs.io/) network), and they will be fetched directly by the [React](https://reactjs.org/)-made frontend.

This will allow to deploys Timariti istances with almost zero web server configuration, but everything is going to be manged in the GitHub repositories, using markdown and JSON files.
