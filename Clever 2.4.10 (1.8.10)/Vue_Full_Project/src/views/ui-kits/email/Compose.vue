<template>
  <div class="animated fadeIn">
    <div class="email-app">
      <nav>
        <a href="#" class="btn btn-danger btn-block">New Email</a>
        <ul class="nav">
          <li class="nav-item">
            <a class="nav-link" href="#"><i class="fa fa-inbox"></i> Inbox <b-badge variant="danger">4</b-badge></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><i class="fa fa-star"></i> Stared</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><i class="fa fa-rocket"></i> Sent</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><i class="fa fa-trash-o"></i> Trash</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><i class="fa fa-bookmark"></i> Important<b-badge variant="info">5</b-badge></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><i class="fa fa-inbox"></i> Inbox <b-badge variant="danger">4</b-badge></a>
          </li>
        </ul>
      </nav>
      <main>
        <p class="text-center">New Message</p>
        <form>
          <div class="form-row mb-3">
            <label for="to" class="col-2 col-sm-1 col-form-label">To:</label>
            <div class="col-10 col-sm-11">
              <input type="email" class="form-control" id="to" placeholder="Type email">
            </div>
          </div>
          <div class="form-row mb-3">
            <label for="cc" class="col-2 col-sm-1 col-form-label">CC:</label>
            <div class="col-10 col-sm-11">
              <input type="email" class="form-control" id="cc" placeholder="Type email">
            </div>
          </div>
          <div class="form-row mb-3">
            <label for="bcc" class="col-2 col-sm-1 col-form-label">BCC:</label>
            <div class="col-10 col-sm-11">
              <input type="email" class="form-control" id="bcc" placeholder="Type email">
            </div>
          </div>
        </form>
        <div class="row">
          <div class="col-sm-11 ml-auto">
            <div class="toolbar" role="toolbar">
              <div class="btn-group">
                <button type="button" class="btn btn-light"><span class="fa fa-bold"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-italic"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-underline"></span></button>
              </div>
              <div class="btn-group">
                <button type="button" class="btn btn-light"><span class="fa fa-align-left"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-align-right"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-align-center"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-align-justify"></span></button>
              </div>
              <div class="btn-group">
                <button type="button" class="btn btn-light"><span class="fa fa-indent"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-outdent"></span></button>
              </div>
              <div class="btn-group">
                <button type="button" class="btn btn-light"><span class="fa fa-list-ul"></span></button>
                <button type="button" class="btn btn-light"><span class="fa fa-list-ol"></span></button>
              </div>
              <button type="button" class="btn btn-light"><span class="fa fa-trash-o"></span></button>
              <button type="button" class="btn btn-light"><span class="fa fa-paperclip"></span></button>
              <div class="btn-group">
                <button type="button" class="btn btn-light dropdown-toggle" data-toggle="dropdown"><span class="fa fa-tags"></span> <span class="caret"></span></button>
                <div class="dropdown-menu">
                  <a class="dropdown-item" href="#">add label <b-badge variant="danger"> Home</b-badge></a>
                  <a class="dropdown-item" href="#">add label <b-badge variant="info"> Job</b-badge></a>
                  <a class="dropdown-item" href="#">add label <b-badge variant="success"> Clients</b-badge></a>
                  <a class="dropdown-item" href="#">add label <b-badge variant="warning"> News</b-badge></a>
                </div>
              </div>
            </div>
            <div class="form-group mt-4">
              <textarea class="form-control" id="message" name="body" rows="12" placeholder="Click here to reply"></textarea>
            </div>
            <div class="form-group">
              <button type="submit" class="btn btn-success">Send</button>
              <button type="submit" class="btn btn-light">Draft</button>
              <button type="submit" class="btn btn-danger">Discard</button>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>
<script>

export default {
  name: 'compose'
}
</script>
