genrule(
  name = 'tree', 
  executable = True, 
  out = 'tree.sh', 
  srcs = [
    'tree.sh', 
  ], 
  cmd = 'cp $SRCS $OUT && chmod +x $OUT', 
)

sh_binary(
  name = 'app', 
  main = ':tree', 
  resources = glob([
    'res/**/*.txt', 
  ]), 
)
