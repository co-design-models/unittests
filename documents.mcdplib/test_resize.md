
<pre class='mcdp' id='compact_example'>
    mcdp {
      a = instance template mcdp {
          provides f [Nat]
          requires r1 [Nat]
          requires r2 [Nat]
      }
      b = instance template mcdp {
          provides f1 [Nat]
          provides f2 [Nat]
          requires r [Nat]
      }
      r1 required by a ≼ f1 provided by b
      r2 required by a ≼ f2 provided by b
    }
</pre>

<render class='ndp_graph_expand'>`compact_example</render>
