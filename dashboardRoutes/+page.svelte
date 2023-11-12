<script>
  import Mainpage from '../../dashboard/mainpage.svelte'
  import Nav from '../../dashboard/nav.svelte'
  import RightSidebar from '../../dashboard/rightSidebar.svelte'
  import Sidebar from '../../dashboard/sidebar.svelte'
</script>

<main>
  <Nav />

  <div class="grid grid-cols-12 gap-x-20">
    <Sidebar />
    <Mainpage />
    <RightSidebar />
  </div>
</main>
