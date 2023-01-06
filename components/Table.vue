<template>
	<div class="container-fluid main-table">
	  <b-navbar toggleable="lg" type="dark" variant="dark">
		<b-navbar-brand href="#"
		  ><img src="../assets/travelshopturkey-logo.png" alt=""
		/></b-navbar-brand>

		<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

		<b-collapse id="nav-collapse" is-nav>
		  <b-navbar-nav>
			<b-nav-item href="#">Home</b-nav-item>
			<b-nav-item href="#">Blog</b-nav-item>
		  </b-navbar-nav>

		  <b-navbar-nav class="ml-auto">
			<b-nav-item-dropdown text="Lang" right>
			  <b-dropdown-item href="#">EN</b-dropdown-item>
			  <b-dropdown-item href="#">ES</b-dropdown-item>
			  <b-dropdown-item href="#">RU</b-dropdown-item>
			  <b-dropdown-item href="#">FA</b-dropdown-item>
			</b-nav-item-dropdown>

			<b-nav-item-dropdown right>
			  <template #button-content>
				<em>User</em>
			  </template>
			  <b-dropdown-item href="#">Profile</b-dropdown-item>
			  <b-dropdown-item href="#">Sign Out</b-dropdown-item>
			</b-nav-item-dropdown>
		  </b-navbar-nav>
		</b-collapse>
	  </b-navbar>
	  <div class="container-fluid">
		<div class="row">
		  <div class="col">
			<table class="table">
			  <thead>
				<tr>
				  <th scope="col">ID</th>
				  <th scope="col">Logo</th>
				  <th scope="col">Name</th>
				  <th scope="col">Settings</th>
				</tr>
			  </thead>
			  <tbody>
				<tr class="colorful">
				  <td scope="row">1</td>
				  <td><img src="../assets/logos/logo1.png" alt="" /></td>
				  <td>Otto</td>
				  <td>
					<button class="btn btn-danger mr-3">
					  <b-icon-trash-fill> </b-icon-trash-fill></button
					><button class="btn btn-primary">
					  <b-icon-pencil-fill></b-icon-pencil-fill>
					</button>
				  </td>
				</tr>
				<tr>
				  <td scope="row">2</td>
				  <td><img src="../assets/logos/logo2.jpg" alt="" /></td>
				  <td>Thornton</td>
				  <td>
					<button class="btn btn-danger mr-3">
					  <b-icon-trash-fill> </b-icon-trash-fill></button
					><button class="btn btn-primary">
					  <b-icon-pencil-fill></b-icon-pencil-fill>
					</button>
				  </td>
				</tr>
				<tr class="colorful">
				  <td scope="row">3</td>
				  <td><img src="../assets/logos/logo3.png" alt="" /></td>
				  <td>Larry</td>
				  <td>
					<button class="btn btn-danger mr-3">
					  <b-icon-trash-fill> </b-icon-trash-fill></button
					><button class="btn btn-primary">
					  <b-icon-pencil-fill></b-icon-pencil-fill>
					</button>
				  </td>
				</tr>
			  </tbody>
			</table>
		  </div>
		</div>
	  </div>
	</div>
  </template>

  <script>
  import { BIconTrashFill, BIconPencilFill } from "bootstrap-vue";

  export default {
	name: "Table",
	components: {
	  BIconTrashFill,
	  BIconPencilFill,
	},
	data() {
	  return {};
	},
  };
  </script>
  <style>
  @import url("https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap");
  .main-table {
	font-family: "Roboto Mono", monospace;
	margin: 0;
	padding: 0;
  }
  th {
	font-size: 1.3em;
  }
  .table th,
  .table td {
	vertical-align: middle !important;
  }
  tr {
	text-align: center;
  }
  tbody {
	text-align: center;
  }
  .colorful {
	background-color: #edf3fd;
  }
  </style>
