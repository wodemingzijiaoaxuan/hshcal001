from building import *
Import('rtconfig')

src= []
cwd= GetCurrentDir()

# add hts221 src files.
src += Glob('sensor_alps_hshcal001.c')
src += Glob('hshcal001.c')
src += Glob('hshcal001_reg.c')

# add hts221 include path.
path= [cwd]

# add src and include to group.
group= DefineGroup('hshcal001', src, depend = ['PKG_USING_HSHCAL001'], CPPPATH = path)

Return('group')

