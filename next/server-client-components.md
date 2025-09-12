if you mark a component with "use-client", everything that is "imported" into that file
will also be a client component, however if you use the `children` prop to pass
a server component to a client component, that component will still be rendered 
on the server. note that both the client component and the server component passed
as the `children` prop need to be inside a server component themselves.
