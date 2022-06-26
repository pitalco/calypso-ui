<script context="module">
	export const prerender = true;
</script>

<script>
    import { Sidebar, SidebarWrapper, SidebarGroup, SidebarItem } from "flowbite-svelte";
    import { ChartPie, ViewGrid, InboxIn, User, Login, Cog } from "svelte-heros";
</script>

<aside class="menu is-vcentered">
    <Sidebar asideClass="black-bg">
        <SidebarWrapper divClass="overflow-y-auto py-4 px-3 bg-black-50 rounded dark:bg-gray-800">
          <SidebarGroup>
            <SidebarItem href="/" label="Dashboard" icon={{ name: ChartPie }} aClass="flex items-center p-2 text-white font-normal hover:text-black rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 no-decoration"/>
            <SidebarItem href="/discover" label="Discover" icon={{ name: User }} aClass="flex items-center p-2 text-white font-normal hover:text-black rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 no-decoration"/>
            <SidebarItem href="/transactions" label="Transactions" icon={{ name: InboxIn }} aClass="flex items-center p-2 text-white font-normal hover:text-black rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 no-decoration"/>
            <SidebarItem href="/airdrop" label="Airdrop" icon={{ name: ViewGrid }} aClass="flex items-center p-2 text-white font-normal hover:text-black rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 no-decoration"/>
            <SidebarItem href="/settings" label="Settings" icon={{ name: Cog }} aClass="flex items-center p-2 text-white font-normal hover:text-black rounded-lg dark:text-white hover:bg-gray-100 dark:hover:bg-gray-700 no-decoration"/>
          </SidebarGroup>
        </SidebarWrapper>
      </Sidebar>
</aside>

<style>
</style>