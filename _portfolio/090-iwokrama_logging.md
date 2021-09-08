---
title: FSC Certification of Reduced-Impact Logging at Iwokrama
image:
 - "/assets/photos/iwokrama_logging/01.jpg"
---

<div class="card-columns">
    {% for image in site.static_files %}
    {% if image.path contains 'assets/photos/iwokrama_logging' %}
    <div class="card" data-toggle="modal" data-target="#exampleModal" data-img="{{ site.baseurl }}{{ image.path }}">
        <img class="card-img-top" src="{{ site.baseurl }}{{ image.path }}" alt="image" />
    </div>
    {% endif %}
    {% endfor %}
</div>

<div class="modal fade" id="exampleModal">
  <div class="modal-dialog modal-lg modal-dialog-centered">
    <div class="modal-content">
      <div class="modal-body">
        <img class="modal-img w-100" />
      </div>
    </div>
  </div>
</div>

<script type="text/javascript">
  $(document).ready(function() {
    $('#exampleModal').on('show.bs.modal', function (event) {
      var button = $(event.relatedTarget)
      var img = button.data('img')
      var modal = $(this)
      modal.find('.modal-img').attr('src', img)
    })
  })
</script>
