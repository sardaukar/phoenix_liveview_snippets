# Phoenix LiveView snippets for Sublime Text

Taken from the Phoenix LiveView course from The Pragmatic Studio.

Place these in a folder and copy it over to `~/.config/sublime-text/Packages`. To be hosted on PackageControl some day.

Included:

- `checkbox` -> `<input type="checkbox" id="${1}" name="${2}" value="${3}"/>`
- `econd` -> ```<%= cond do %>
  <% $1 -> %>
    $2
  <% true -> %>
    $3
<% end %>```
- `data` -> ```<datalist id="${1}">
  ${0}
</datalist>```
- `eelse` -> `<% else %>`
- `eend` -> `% end %>`
- `hidden` -> ```<input type="hidden" name="${1}" value="${2}" />```
- `eif` -> ```<%= if $1 do %>
  $2
<% end %>```
- `eife` -> ```<%= if $1 do %>
  $2
<% else %>
  $3
<% end %>```
- `eifa` -> ```<%= if $1, do: "{$1}" %>```
- `input` -> ```<input type="text" name="${1}" value="${2}"
       placeholder="${3}" />```
- `et` -> ```<%= $1 %>```
- `eunless` -> ```%= unless $1 do %>
  $2
<% end %>```
- `efor` -> ```<%= for ${1:item} <- @$1s do %>
  $2
<% end %>```
- `efori` -> ```<%= for ${1:item} <- @$1s do %>
  $2
<% end %>```
- `lc` -> ```defmodule LiveViewStudioWeb.${1}Component do
  use LiveViewStudioWeb, :live_component
end]```
- `he` -> ```def handle_event(${1:event}, _, socket) do
  socket = assign(socket, ${2:key}: ${3:value})
  {:noreply, socket}
end```
- `hi` -> ```def handle_info(${1:message}, socket) do
  socket = assign(socket, ${2:key}: ${3:value})
  {:noreply, socket}
end```
- `hp` -> ```def handle_params(params, _url, socket) do
  {:noreply, socket}
end```
- `lv` -> ```defmodule LiveViewStudioWeb.${1}Live do
  use LiveViewStudioWeb, :live_view
end```
- `mount` -> ```def mount(_params, _session, socket) do
  socket = assign(socket, ${1:key}: ${2:value})
  {:ok, socket}
end```
- `rend` -> ```def render(assigns) do
  ~L"""
  ${0}
  """
end```
- `lt` -> ```~L"""
${0}
"""```
- `test` -> ```test "${1:description}", %{conn: conn} do
  {:ok, view, _html} = live(conn, "${2:path}")
  ${0}
end```
- `lvtest` -> ```defmodule LiveViewStudioWeb.${1}Test do
  use LiveViewStudioWeb.ConnCase, async: true
  import Phoenix.LiveViewTest
  ${0}
end```


Pull requests for improvements welcome.
