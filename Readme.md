
# uncollapse

  CSS utility for undoing css margin collapsing

 - This utility class prevents decendents from margin collapsing
 - The technique is an evolution upon http://stackoverflow.com/questions/1828804/how-do-i-uncollapse-a-margin

## Installation

    $ component install jasonkuhrt/uncollapse

## API

    .uncollapse

  Apply this class on a container whose descendents' margin-top's are protruding beyond its bounds

## Example

    <!-- The problem -->
    <article>
      <div style="background-color:grey;">
        <h1>Demo</h1>
      </div>
      <div style="background-color:red;">
        <p style="margin:32px;">Oops, notice I don't make my container 64px tall!</p>
      </div>
    </article>



    <!-- The solution -->
    <article>
      <div style="background-color:grey;">
        <h1>Demo</h1>
      </div>
      <div class="uncollapse" style="background-color:red;">
        <p style="margin:32px;">Oops, notice I don't make my container 64px tall!</p>
      </div>
    </article>

## License

  MIT
