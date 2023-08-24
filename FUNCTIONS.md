# os

os.MkdirTemp
os.CreateTemp
os.ReadDir
os.Stat
os.Truncate
os.OpenFile(
		path.Join(dir, fmt.Sprintf("%d%s", baseOffset, ".store")),
		os.O_RDWR|os.O_CREATE|os.O_APPEND,
		0644,
	)
os.Remove
os.RemoveAll

# os.File

s.File.ReadAt(b, int64(pos+lenWidth))

# mutex

sync.RWMutex
sync.Mutex
mu.RLock()
mu.RUnlock()

# binary

binary.BigEndian.Uint32
binary.BigEndian.Uint64
binary.BigEndian.PutUint32
binary.BigEndian.PutUint64
binary.Write(s.buf, enc, uint64(len(p)))

# bufio

bufio.Writer
bufio.NewWriter(f)
buf.Flush()
buf.Write(p)

# gommap

gommap.Map(idx.file.Fd(), gommap.PROT_READ|gommap.PROT_WRITE, gommap.MAP_SHARED)
i.mmap.Sync(gommap.MS_SYNC)

# proto

proto.Marshal
proto.Unmarshal

# strings

strings.TrimSuffix

# strconv

strconv.ParseUint
strconv.FormatUint
strconv.Itoa

# sort

sort.Slice(baseOffsets, func(i, j int) bool {
		return baseOffsets[i] < baseOffsets[j]
	})


# io

io.Reader
io.MultiReader

# testing

t.Run
t.Helper()

# testify

require.Equal
require.NotEqual
require.Nil
require.Error
require.NoError
require.True
require.False
