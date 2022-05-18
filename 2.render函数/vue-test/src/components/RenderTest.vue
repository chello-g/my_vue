<script>
export default {
  name: "HelloWorld",
  props: {
    tag: String,
  },
  data() {
    return {
      peopleList: ["张三1", "张三2", "张三3"],
    };
  },
  render(createElement) {
    return createElement(
      this.tag,
      {},
      this.peopleList.map((name) => createElement("li", {attrs:{class:"custom-text"}}, name))
    );
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.custom-text{
  color:cadetblue;
}
</style>
