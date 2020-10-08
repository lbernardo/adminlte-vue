# adminlte-vue
Use https://adminlte.io/ with VueJS

### Example

```js
<template>
  <Container>
    <Navbar />  
    <Sidebar>
      <div class="user-panel mt-3 pb-3 mb-3 d-flex">
        <div class="image">
          <img src="dist/img/user2-160x160.jpg" class="img-circle elevation-2" alt="User Image">
        </div>
        <div class="info">
          <a href="#" class="d-block">Alexander Pierce</a>
        </div>
      </div>
      <Menubar>
        <MenubarItem text="Dashboard" icon="fas fa-chart-pie" />
      </Menubar>
    </Sidebar>
    <Content title="Dashboard" :breadcrumb="['Home', 'Dashboard']" />
  </Container>
</template>

<script>
import {
  Container, 
  Navbar, 
  Sidebar, 
  Menubar, 
  MenubarItem,
  Content,
} from 'adminlte-vue';

export default {
  name: 'App',
  components: {
    Container,
    Navbar,
    Sidebar,
    Menubar,
    MenubarItem,
    Content
  }
}
</script>
```