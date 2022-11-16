<script>
  import { Router, Route } from 'svelte-routing'
  import Home from '../pages/Home.svelte'
  import Blog from '../pages/Blog.svelte'
  import About from '../pages/About.svelte'

  export let url = ''
</script>

<Router {url}>
  <Route path="blog" component={Blog} />
  <Route path="about" component={About} />
  <Route path="/" component={Home} />
</Router>