# Partial view toggle control

With the partial view toggle control, you can toggle between different [partial views](/guides/partial-views.html).

<p class="alert alert-info">
  Wondering how to set up a partial views for your control? Check out <a href="/guides/partial-views.html">our full guide on partial views</a>.
</p>

![view toggle gif](/images/view-toggle.gif)

Here's the syntax for adding the view toggle control in the Advanced Editor:

```
@controls {
  top {
    view-toggle {}
  }
}
```

You can use the `options` property inside the control to list exactly which partial views should be included as options:

```
@controls {
  top {
    view-toggle {
      options: "one-partial", "another-partial", "a-third-partial";
    }
  }
}
```

You can also use the `option {}` syntax if you'd like to customize the list of options _and_ how they're labelled on the map:

```
@controls {
  top {
    view-toggle {
      option {
        value: "one-partial";
        label: "Toggle first view";
      }

      option {
        value: "another-partial";
        label: "Toggle second view";
      }

      option {
        value: "a-third-partial";
        label: "Toggle third view";
      }
    }
  }
}
```

[Check out our controls reference](/guides/controls/controls-reference.md) to see the full list of properties and values recognized by the view-toggle control.

<span class="edit-link"><a href="https://github.com/kumu/docs/blob/master/guides/controls/view-toggle-control.md" target="_blank"><i class="fa fa-github"></i> edit this page</a></span>