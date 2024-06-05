#let rec hanoi n i j =
 if n > 0 then begin
  hanoi (n - 1) i (6 - (i + j));
  Printf.printf "%d -> %d\n" i j;
  hanoi (n - 1) (6 - (i + j)) j;
 end;;
