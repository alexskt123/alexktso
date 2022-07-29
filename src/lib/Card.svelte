<script>
  import { Card, CardText, CardActions, Button, MaterialApp } from 'svelte-materialify';
</script>

<MaterialApp>
  <div class="d-flex justify-center mt-4 mb-4">
    <Card outlined style="max-width:300px;">
      <div class="pl-4 pr-4 pt-3">
        <span class="text-h5 mb-2">StockIsFun</span>
      </div>
      <CardText>
        A website built with Nextjs and Firebase to study Stock
      </CardText>
      <CardActions>
        <Button rounded outlined>Link</Button>
      </CardActions>
    </Card>
  </div>
</MaterialApp>
